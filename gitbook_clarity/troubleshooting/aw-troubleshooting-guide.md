---
description: "A+W Software - Troubleshooting Guide"
---


# A+W Software - Troubleshooting Guide

This guide provides solutions to common issues encountered with A+W software, derived from analysis of real support cases.

## Installation Issues

### Issue: Installation fails with "Missing dependencies" error

**Symptoms:**
- Setup launcher reports missing components
- Installation cannot proceed

**Solutions:**
1. Verify all prerequisites are installed:
   - .NET Framework 4.7.2 or later
   - Visual C++ Redistributables
   - SQL Server Client Tools
2. Run Windows Update to ensure system is current
3. Check Windows Event Viewer for detailed error messages
4. Run installer as Administrator
5. Temporarily disable antivirus software

**Related Documentation:** Installation Instructions for specific modules

### Issue: Database connection fails during installation

**Symptoms:**
- Cannot connect to SQL Server
- "Login failed" or "Server not found" errors

**Solutions:**
1. Verify SQL Server is running
2. Check SQL Server authentication mode (Windows/Mixed)
3. Confirm firewall allows SQL Server port (default 1433)
4. Test connection with SQL Server Management Studio
5. Verify user has appropriate database permissions
6. Check connection string syntax

### Issue: License activation fails

**Symptoms:**
- "Invalid license" error
- Cannot activate product

**Solutions:**
1. Verify license key is correct (check for typos)
2. Ensure system clock is accurate
3. Check internet connectivity for online activation
4. Verify hardware ID matches license
5. Contact A+W support for license file
6. Check for conflicting license managers

## Configuration Issues

### Issue: Module not appearing in interface

**Symptoms:**
- Expected functionality is missing
- Menu items not visible

**Solutions:**
1. Verify module is installed
2. Check user rights and permissions
3. Review EDP Module Codes configuration
4. Restart application and services
5. Clear application cache
6. Verify license includes the module

### Issue: Data not synchronizing between modules

**Symptoms:**
- Changes in one module not reflected in another
- Stale or outdated data

**Solutions:**
1. Check A+W SOA services are running
2. Verify network connectivity between components
3. Review synchronization settings
4. Check for database locks or deadlocks
5. Verify data replication configuration
6. Review error logs for sync failures

### Issue: Printer configuration not working

**Symptoms:**
- Labels or documents not printing
- Wrong printer selected

**Solutions:**
1. Verify printer is installed and online
2. Check printer driver compatibility
3. Review printer mapping configuration
4. Test with Windows test page
5. Check application printer settings
6. Verify user has printer permissions

## Production Issues

### Issue: Optimization not finding solutions

**Symptoms:**
- Optimizer returns no results
- "No valid solution" message

**Solutions:**
1. Review material dimensions and constraints
2. Check stock availability
3. Verify optimization parameters
4. Reduce constraint complexity
5. Check for conflicting rules
6. Review defect definitions
7. Increase optimization time limit

### Issue: Machine not receiving jobs

**Symptoms:**
- Production data not transferring to machine
- Machine shows "No jobs" or "Waiting"

**Solutions:**
1. Verify machine client is running
2. Check network connectivity to machine
3. Review machine allocation settings
4. Confirm job is released for production
5. Check machine status and availability
6. Review production schedule
7. Verify machine interface configuration

### Issue: Barcode scanning not working

**Symptoms:**
- Scanner not reading barcodes
- Wrong data captured

**Solutions:**
1. Verify scanner is properly connected
2. Check scanner configuration and symbology settings
3. Test scanner with known good barcode
4. Verify barcode format matches expected format
5. Check for damaged or dirty barcodes
6. Review application barcode settings
7. Ensure scanner driver is installed

## Performance Issues

### Issue: System running slowly

**Symptoms:**
- Long response times
- Timeouts
- Unresponsive interface

**Solutions:**
1. Check database performance:
   - Review query execution plans
   - Update statistics
   - Rebuild indexes
   - Check for blocking queries
2. Review system resources:
   - CPU usage
   - Memory utilization
   - Disk I/O
   - Network bandwidth
3. Optimize application settings:
   - Reduce data range in queries
   - Adjust cache settings
   - Limit concurrent users
4. Check for:
   - Antivirus scanning interference
   - Windows updates running
   - Backup operations
   - Other resource-intensive processes

### Issue: Database growing too large

**Symptoms:**
- Disk space warnings
- Slow database operations
- Backup failures

**Solutions:**
1. Implement data archiving strategy
2. Purge old transaction data
3. Review log file growth settings
4. Compress old data
5. Move archived data to separate database
6. Adjust database maintenance plans
7. Consider database partitioning

## Integration Issues

### Issue: B2B orders not importing

**Symptoms:**
- Import process fails
- Orders incomplete or incorrect

**Solutions:**
1. Verify file format matches specification
2. Check for XML/data validation errors
3. Review import log files
4. Verify customer master data exists
5. Check product mapping configuration
6. Ensure file permissions allow access
7. Test with sample file

### Issue: CAD data not transferring

**Symptoms:**
- Shapes not importing
- Dimension errors

**Solutions:**
1. Verify CAD file format compatibility
2. Check unit of measurement settings
3. Review shape complexity limits
4. Validate CAD data integrity
5. Check for unsupported features
6. Verify CAD service is running
7. Test with simple shapes first

### Issue: Financial data export failing

**Symptoms:**
- Export process errors
- Incomplete data in accounting system

**Solutions:**
1. Verify export format configuration
2. Check date range and filters
3. Review mapping of accounts and cost centers
4. Ensure all required fields are populated
5. Check for special characters in data
6. Verify file path and permissions
7. Test export with small dataset

## Mobile App Issues

### Issue: Smart Companion not connecting

**Symptoms:**
- "Cannot connect to server" error
- App shows offline

**Solutions:**
1. Verify mobile device has network connectivity
2. Check WiFi or cellular data connection
3. Confirm server URL is correct
4. Verify firewall allows mobile access
5. Check SSL certificate validity
6. Test connection from web browser
7. Restart app and mobile device

### Issue: Barcode scanning in app not working

**Symptoms:**
- Camera not activating
- Barcodes not recognized

**Solutions:**
1. Grant camera permissions to app
2. Ensure adequate lighting
3. Hold device steady at correct distance
4. Clean camera lens
5. Verify barcode format is supported
6. Test with known good barcode
7. Update app to latest version

## Error Messages

### "Connection timeout"

**Causes:**
- Network issues
- Server overload
- Firewall blocking

**Solutions:**
- Check network connectivity
- Verify server is responding
- Review firewall rules
- Increase timeout settings
- Check for network congestion

### "Access denied"

**Causes:**
- Insufficient permissions
- Incorrect credentials
- Expired password

**Solutions:**
- Verify user credentials
- Check user rights configuration
- Reset password if needed
- Review security group membership
- Contact administrator

### "Database deadlock detected"

**Causes:**
- Concurrent transactions
- Lock escalation
- Long-running queries

**Solutions:**
- Retry operation
- Review transaction isolation levels
- Optimize query performance
- Reduce transaction scope
- Implement retry logic

### "Service unavailable"

**Causes:**
- Service not running
- Server maintenance
- Resource exhaustion

**Solutions:**
- Check service status
- Restart required services
- Review system resources
- Check for scheduled maintenance
- Review error logs

## Diagnostic Tools

### Log File Locations

- **Application Logs:** `C:\ProgramData\A+W\Logs\`
- **Service Logs:** `C:\Program Files\A+W\[Service]\Logs\`
- **IIS Logs:** `C:\inetpub\logs\LogFiles\`
- **Windows Event Viewer:** Application and System logs

### Useful Commands

```
# Check service status
Get-Service -Name "A+W*"

# Test network connectivity
Test-NetConnection -ComputerName [server] -Port [port]

# Check SQL Server connectivity
sqlcmd -S [server] -U [user] -P [password]

# View recent errors in Event Viewer
Get-EventLog -LogName Application -Newest 50 -EntryType Error
```

### Performance Monitoring

- **Task Manager:** Quick resource overview
- **Resource Monitor:** Detailed resource usage
- **Performance Monitor:** Long-term performance tracking
- **SQL Server Profiler:** Database query analysis
- **Network Monitor:** Network traffic analysis

## Getting Help

If you cannot resolve an issue using this guide:

1. **Check Documentation:** Review relevant user manuals and configuration guides
2. **Search Knowledge Base:** Look for similar issues in the support portal
3. **Collect Information:**
   - Detailed error messages
   - Screenshots
   - Log files
   - Steps to reproduce
   - System configuration
4. **Contact Support:**
   - Submit ticket through customer portal
   - Email: support@a-w.com
   - Include all collected information

## Preventive Maintenance

To minimize issues:

- **Regular Updates:** Apply patches and updates promptly
- **Database Maintenance:** Schedule regular index rebuilds and statistics updates
- **Backup Strategy:** Implement comprehensive backup plan
- **Monitor Performance:** Track key metrics and trends
- **User Training:** Ensure users understand proper procedures
- **Documentation:** Keep configuration documentation current
- **Testing:** Test changes in non-production environment first

---

*This troubleshooting guide is based on real support cases and is regularly updated with new solutions.*
