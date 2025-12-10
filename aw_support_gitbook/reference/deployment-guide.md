---
title: "A+W Support AI Assistant - Deployment Guide"
category: "documentation"
product: "A+W Software"
doc_type: "Deployment Guide"
language: "EN"
tags: ["deployment", "openai", "setup", "configuration"]
version: "1.0"
last_updated: "2025-12-10"
description: "Complete deployment guide for setting up the A+W Support AI Assistant with OpenAI API"
---

# A+W Support AI Assistant - Deployment Guide

This guide provides step-by-step instructions for deploying the A+W Support AI Assistant using OpenAI's API and vector store.

---

## Prerequisites

### Required

- OpenAI API account with access to:
  - GPT-4 Turbo or GPT-4
  - Assistants API (Beta)
  - File Search / Vector Store capabilities
- Python 3.8+ (for deployment scripts)
- OpenAI Python SDK 1.0+

### Recommended

- API usage monitoring tools
- Backup storage for knowledge base
- Version control system (Git)

---

## Step 1: Prepare the Knowledge Base

### 1.1 Extract the Knowledge Base

```bash
# Extract the knowledge base archive
tar -xzf aw_support_kb_complete.tar.gz

# Verify contents
cd aw_support_kb
ls -la

# Expected output:
# 00_MASTER_INDEX.md
# README.md
# PRODUCT_INDEX.md
# DEPLOYMENT_GUIDE.md
# 01_installation/
# 02_configuration/
# 03_user_manuals/
# ... (remaining directories)
```

### 1.2 Verify File Count

```bash
# Count total markdown files
find . -name "*.md" | wc -l
# Expected: 1,348 files
```

### 1.3 Review Key Documents

Before deployment, review:
- `00_MASTER_INDEX.md` - Complete taxonomy
- `README.md` - Usage instructions
- `PRODUCT_INDEX.md` - Product reference
- `DEPLOYMENT_GUIDE.md` - This file

---

## Step 2: Install Dependencies

### 2.1 Install OpenAI SDK

```bash
pip install openai
```

### 2.2 Verify Installation

```python
import openai
print(openai.__version__)
# Should be 1.0.0 or higher
```

---

## Step 3: Upload to Vector Store

### 3.1 Create Upload Script

Save as `upload_knowledge_base.py`:

```python
#!/usr/bin/env python3
"""
Upload A+W Support Knowledge Base to OpenAI Vector Store
"""

from openai import OpenAI
from pathlib import Path
import time

# Configuration
API_KEY = "your-openai-api-key-here"
KB_PATH = Path("aw_support_kb")
VECTOR_STORE_NAME = "A+W Support Knowledge Base"

# Initialize client
client = OpenAI(api_key=API_KEY)

def upload_knowledge_base():
    """Upload all markdown files to vector store"""
    
    print("=" * 60)
    print("A+W Support Knowledge Base Upload")
    print("=" * 60)
    
    # Get all markdown files
    md_files = list(KB_PATH.rglob("*.md"))
    print(f"\nFound {len(md_files)} markdown files")
    
    # Create vector store
    print(f"\nCreating vector store: {VECTOR_STORE_NAME}")
    vector_store = client.beta.vector_stores.create(
        name=VECTOR_STORE_NAME,
        expires_after={
            "anchor": "last_active_at",
            "days": 365  # Keep for 1 year
        }
    )
    print(f"✓ Vector store created: {vector_store.id}")
    
    # Upload files in batches (OpenAI limit: 500 files per batch)
    batch_size = 500
    total_batches = (len(md_files) + batch_size - 1) // batch_size
    
    print(f"\nUploading {len(md_files)} files in {total_batches} batch(es)...")
    
    for i in range(0, len(md_files), batch_size):
        batch_files = md_files[i:i + batch_size]
        batch_num = (i // batch_size) + 1
        
        print(f"\nBatch {batch_num}/{total_batches}: Uploading {len(batch_files)} files...")
        
        try:
            # Open files for upload
            file_streams = [open(file_path, "rb") for file_path in batch_files]
            
            # Upload batch
            file_batch = client.beta.vector_stores.file_batches.upload_and_poll(
                vector_store_id=vector_store.id,
                files=file_streams
            )
            
            # Close file streams
            for stream in file_streams:
                stream.close()
            
            print(f"✓ Batch {batch_num} uploaded successfully")
            print(f"  Status: {file_batch.status}")
            print(f"  File counts: {file_batch.file_counts}")
            
        except Exception as e:
            print(f"✗ Error uploading batch {batch_num}: {e}")
            # Close any open streams
            for stream in file_streams:
                try:
                    stream.close()
                except:
                    pass
    
    # Verify upload
    print("\nVerifying upload...")
    time.sleep(2)  # Wait for processing
    
    vector_store = client.beta.vector_stores.retrieve(vector_store.id)
    print(f"\n✓ Upload complete!")
    print(f"  Vector Store ID: {vector_store.id}")
    print(f"  Total files: {vector_store.file_counts.completed}")
    print(f"  Status: {vector_store.status}")
    
    return vector_store.id

if __name__ == "__main__":
    vector_store_id = upload_knowledge_base()
    print(f"\n{'=' * 60}")
    print("IMPORTANT: Save this Vector Store ID:")
    print(f"  {vector_store_id}")
    print("=" * 60)
```

### 3.2 Run Upload Script

```bash
# Set your API key
export OPENAI_API_KEY="your-api-key-here"

# Run upload
python upload_knowledge_base.py

# Save the Vector Store ID from the output
```

**Expected Output:**
```
============================================================
A+W Support Knowledge Base Upload
============================================================

Found 1348 markdown files

Creating vector store: A+W Support Knowledge Base
✓ Vector store created: vs_abc123...

Uploading 1348 files in 3 batch(es)...

Batch 1/3: Uploading 500 files...
✓ Batch 1 uploaded successfully
...

✓ Upload complete!
  Vector Store ID: vs_abc123...
  Total files: 1348
  Status: completed

============================================================
IMPORTANT: Save this Vector Store ID:
  vs_abc123...
============================================================
```

---

## Step 4: Create the AI Assistant

### 4.1 Create Assistant Script

Save as `create_assistant.py`:

```python
#!/usr/bin/env python3
"""
Create A+W Support AI Assistant
"""

from openai import OpenAI

# Configuration
API_KEY = "your-openai-api-key-here"
VECTOR_STORE_ID = "vs_abc123..."  # From Step 3

# Initialize client
client = OpenAI(api_key=API_KEY)

# Assistant instructions
INSTRUCTIONS = """You are an expert A+W Software support assistant with comprehensive knowledge of all A+W products including Enterprise, Business, Production, Clarity, Smart Factory, Smart Companion, Analytics, and iShape.

Your knowledge base contains:
- 1,348 documents covering installation, configuration, user manuals, and troubleshooting
- Documentation in English and German
- Support ticket analysis from 2,888 real customer cases
- FAQs and common issue resolutions

When responding to questions:

1. **Search thoroughly:** Use file search to find relevant documentation
2. **Cite sources:** Reference specific documents by title and category
3. **Be specific:** Provide exact steps, parameters, and configuration details
4. **Structure responses:** Use clear headings, numbered steps, and formatting
5. **Provide context:** Explain why solutions work, not just what to do
6. **Suggest alternatives:** Offer multiple approaches when applicable
7. **Cross-reference:** Point to related documentation for deeper understanding
8. **Acknowledge limitations:** If information is incomplete, say so clearly

Response Format:
- Start with a direct answer to the question
- Provide step-by-step instructions when applicable
- Include relevant warnings or prerequisites
- Cite document sources in format: [Document Title] (Category)
- Suggest related topics or next steps

Language Handling:
- Respond in the user's query language (English or German)
- For German queries, prioritize German documentation (language: DE)
- For English queries, prioritize English documentation (language: EN)

Escalation Criteria:
Recommend contacting A+W support (support@a-w.com) when:
- No relevant documentation exists
- Issue requires system-specific diagnosis
- Problem involves critical production systems
- Custom development or configuration is needed
- User reports a potential bug

Product Knowledge:
- A+W Enterprise: ERP for order management, sales, purchasing
- A+W Business: Pricing, product management, financial integration
- A+W Production: Manufacturing, optimization, capacity planning
- A+W Clarity: Modern web interface for Enterprise
- A+W Smart Factory: Industry 4.0 automation and machine integration
- A+W Smart Companion: Mobile apps (Stock, Dispatch, Production)
- A+W Analytics: Qlik Sense-based BI and reporting
- A+W iShape: CAD software for window/door design

Always be professional, accurate, and helpful. Your goal is to resolve issues quickly while educating users about A+W software capabilities."""

def create_assistant():
    """Create the A+W Support AI Assistant"""
    
    print("Creating A+W Support AI Assistant...")
    
    assistant = client.beta.assistants.create(
        name="A+W Support AI Assistant",
        instructions=INSTRUCTIONS,
        model="gpt-4-turbo-preview",
        tools=[{"type": "file_search"}],
        tool_resources={
            "file_search": {
                "vector_store_ids": [VECTOR_STORE_ID]
            }
        }
    )
    
    print(f"✓ Assistant created successfully!")
    print(f"  Assistant ID: {assistant.id}")
    print(f"  Name: {assistant.name}")
    print(f"  Model: {assistant.model}")
    print(f"  Vector Store: {VECTOR_STORE_ID}")
    
    return assistant.id

if __name__ == "__main__":
    assistant_id = create_assistant()
    print(f"\n{'=' * 60}")
    print("IMPORTANT: Save this Assistant ID:")
    print(f"  {assistant_id}")
    print("=" * 60)
```

### 4.2 Run Assistant Creation

```bash
python create_assistant.py
```

**Expected Output:**
```
Creating A+W Support AI Assistant...
✓ Assistant created successfully!
  Assistant ID: asst_xyz789...
  Name: A+W Support AI Assistant
  Model: gpt-4-turbo-preview
  Vector Store: vs_abc123...

============================================================
IMPORTANT: Save this Assistant ID:
  asst_xyz789...
============================================================
```

---

## Step 5: Test the Assistant

### 5.1 Create Test Script

Save as `test_assistant.py`:

```python
#!/usr/bin/env python3
"""
Test A+W Support AI Assistant
"""

from openai import OpenAI
import time

# Configuration
API_KEY = "your-openai-api-key-here"
ASSISTANT_ID = "asst_xyz789..."  # From Step 4

# Initialize client
client = OpenAI(api_key=API_KEY)

def test_assistant(question):
    """Test the assistant with a question"""
    
    print(f"\nQuestion: {question}")
    print("-" * 60)
    
    # Create thread
    thread = client.beta.threads.create()
    
    # Add message
    message = client.beta.threads.messages.create(
        thread_id=thread.id,
        role="user",
        content=question
    )
    
    # Run assistant
    run = client.beta.threads.runs.create_and_poll(
        thread_id=thread.id,
        assistant_id=ASSISTANT_ID
    )
    
    # Get response
    if run.status == "completed":
        messages = client.beta.threads.messages.list(thread_id=thread.id)
        response = messages.data[0].content[0].text.value
        print(f"\nAnswer:\n{response}")
        
        # Show citations if available
        annotations = messages.data[0].content[0].text.annotations
        if annotations:
            print(f"\n\nSources cited: {len(annotations)}")
    else:
        print(f"Error: Run status is {run.status}")

# Test questions
test_questions = [
    "How do I install A+W Clarity Experience?",
    "What are the system requirements for A+W Enterprise?",
    "How does the Defect Optimizer work?",
    "How do I configure user rights?",
    "What is A+W Smart Factory?"
]

if __name__ == "__main__":
    print("=" * 60)
    print("Testing A+W Support AI Assistant")
    print("=" * 60)
    
    for question in test_questions:
        test_assistant(question)
        print("\n" + "=" * 60)
        time.sleep(2)  # Rate limiting
```

### 5.2 Run Tests

```bash
python test_assistant.py
```

---

## Step 6: Deploy to Production

### 6.1 Integration Options

#### Option A: Web Interface
Create a web application using Flask or FastAPI:

```python
from flask import Flask, request, jsonify
from openai import OpenAI

app = Flask(__name__)
client = OpenAI(api_key="your-api-key")
ASSISTANT_ID = "asst_xyz789..."

@app.route('/ask', methods=['POST'])
def ask_question():
    question = request.json.get('question')
    
    # Create thread and get response
    thread = client.beta.threads.create()
    message = client.beta.threads.messages.create(
        thread_id=thread.id,
        role="user",
        content=question
    )
    run = client.beta.threads.runs.create_and_poll(
        thread_id=thread.id,
        assistant_id=ASSISTANT_ID
    )
    
    if run.status == "completed":
        messages = client.beta.threads.messages.list(thread_id=thread.id)
        response = messages.data[0].content[0].text.value
        return jsonify({"answer": response})
    
    return jsonify({"error": "Failed to get response"}), 500

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)
```

#### Option B: Slack Bot
Integrate with Slack using Bolt framework

#### Option C: Microsoft Teams Bot
Use Bot Framework SDK

#### Option D: Custom Portal
Embed in existing customer support portal

### 6.2 Security Considerations

- **API Key Protection:** Store API keys in environment variables or secrets manager
- **Rate Limiting:** Implement rate limiting to prevent abuse
- **Authentication:** Require user authentication before accessing assistant
- **Logging:** Log all queries and responses for audit and improvement
- **Data Privacy:** Ensure compliance with data protection regulations

### 6.3 Monitoring

Monitor the following metrics:
- Query volume and patterns
- Response times
- Token usage and costs
- User satisfaction ratings
- Common unanswered questions
- Error rates

---

## Step 7: Maintenance and Updates

### 7.1 Regular Updates

**Monthly:**
- Review unanswered questions
- Update FAQ based on new support tickets
- Add new product documentation

**Quarterly:**
- Analyze support ticket trends
- Update troubleshooting guides
- Refresh website content

**With Each Software Release:**
- Add new product documentation
- Update installation guides
- Revise configuration instructions

### 7.2 Update Process

```bash
# 1. Update local knowledge base
cd aw_support_kb
# Add/update markdown files

# 2. Create new vector store
python upload_knowledge_base.py

# 3. Update assistant with new vector store
python update_assistant.py --vector-store-id vs_new123...

# 4. Test updated assistant
python test_assistant.py

# 5. Deploy to production
```

### 7.3 Version Control

Maintain version control for:
- Knowledge base files (Git)
- Deployment scripts
- Assistant configurations
- Update history

---

## Troubleshooting Deployment

### Issue: Upload Fails

**Symptoms:** File upload errors, timeouts

**Solutions:**
- Check API key validity
- Verify file formats (must be .md)
- Reduce batch size
- Check file size limits (512 MB per file)
- Ensure stable internet connection

### Issue: Assistant Not Finding Information

**Symptoms:** "I don't have information about that"

**Solutions:**
- Verify vector store is attached to assistant
- Check file upload completed successfully
- Review query phrasing
- Ensure relevant documents exist in knowledge base
- Check document metadata and tags

### Issue: Slow Response Times

**Symptoms:** Long wait times for responses

**Solutions:**
- Use GPT-4 Turbo (faster than GPT-4)
- Optimize query complexity
- Implement caching for common questions
- Consider response streaming

### Issue: High Costs

**Symptoms:** Unexpected API costs

**Solutions:**
- Monitor token usage
- Implement query length limits
- Cache common responses
- Use GPT-3.5 Turbo for simple queries
- Set spending limits in OpenAI dashboard

---

## Cost Estimation

### Vector Store Costs
- **Storage:** $0.10 per GB per day
- **Estimated KB size:** 22 MB = 0.022 GB
- **Monthly cost:** ~$0.07

### API Usage Costs (GPT-4 Turbo)
- **Input:** $10 per 1M tokens
- **Output:** $30 per 1M tokens
- **Average query:** ~2,000 input + 500 output tokens
- **Cost per query:** ~$0.035

### Estimated Monthly Costs
- 1,000 queries/month: ~$35
- 5,000 queries/month: ~$175
- 10,000 queries/month: ~$350

---

## Support and Resources

### OpenAI Documentation
- [Assistants API Guide](https://platform.openai.com/docs/assistants)
- [File Search Documentation](https://platform.openai.com/docs/assistants/tools/file-search)
- [Vector Stores](https://platform.openai.com/docs/assistants/tools/file-search/vector-stores)

### A+W Resources
- **Support Email:** support@a-w.com
- **Customer Portal:** [A+W Customer Portal]
- **Documentation:** See knowledge base

### Deployment Support
For assistance with deployment:
- Contact A+W Digital Innovation Team
- Review OpenAI community forums
- Consult OpenAI support

---

## Checklist

Before going live, verify:

- [ ] Knowledge base uploaded successfully (1,348 files)
- [ ] Vector store created and active
- [ ] Assistant created with correct configuration
- [ ] Test queries returning accurate responses
- [ ] API keys secured in environment variables
- [ ] Rate limiting implemented
- [ ] User authentication configured
- [ ] Monitoring and logging enabled
- [ ] Backup of knowledge base maintained
- [ ] Update process documented
- [ ] Support team trained on system
- [ ] Escalation procedures defined

---

**Deployment Version:** 1.0  
**Last Updated:** December 10, 2025  
**Next Review:** March 10, 2026

*For questions about this deployment guide, contact A+W Digital Innovation Team*
