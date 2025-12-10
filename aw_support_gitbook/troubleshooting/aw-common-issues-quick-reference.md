---
description: "A+W Software - Common Issues Quick Reference"
---


# A+W Software - Common Issues Quick Reference

Quick solutions to the most frequently encountered issues.

## Top 10 Most Common Issues

### 1. Cannot Connect to Database
**Quick Fix:** Verify SQL Server service is running, check connection string, confirm firewall allows port 1433

### 2. Module Not Visible in Interface
**Quick Fix:** Check user rights, verify module license, restart application

### 3. Printer Not Working
**Quick Fix:** Verify printer is online, check printer mapping, test with Windows test page

### 4. Slow Performance
**Quick Fix:** Rebuild database indexes, check system resources, reduce query date ranges

### 5. Optimization Returns No Results
**Quick Fix:** Review material constraints, check stock availability, verify optimization parameters

### 6. Barcode Scanner Not Reading
**Quick Fix:** Test scanner with known barcode, check scanner configuration, verify barcode format

### 7. Import Process Failing
**Quick Fix:** Validate file format, check for data errors, review import logs

### 8. Mobile App Cannot Connect
**Quick Fix:** Verify network connectivity, check server URL, confirm firewall settings

### 9. Report Not Generating
**Quick Fix:** Check date range, verify data exists, review report parameters

### 10. License Activation Failed
**Quick Fix:** Verify license key, check system clock, ensure internet connectivity

## Quick Diagnostic Checklist

When encountering any issue, check:

- [ ] Are all A+W services running?
- [ ] Is there network connectivity?
- [ ] Are there recent error messages in logs?
- [ ] Has anything changed recently (updates, configuration)?
- [ ] Can the issue be reproduced?
- [ ] Does it affect all users or just one?
- [ ] Is there adequate disk space?
- [ ] Are system resources (CPU, RAM) available?

## Emergency Contacts

- **Support Portal:** [A+W Customer Portal]
- **Email:** support@a-w.com
- **Critical Issues:** Contact your regional A+W office

## Most Useful Log Files

1. `C:\ProgramData\A+W\Logs\[Application].log`
2. Windows Event Viewer → Application
3. SQL Server Error Log
4. IIS Logs (for web services)

---

*For detailed troubleshooting steps, see the complete Troubleshooting Guide.*
