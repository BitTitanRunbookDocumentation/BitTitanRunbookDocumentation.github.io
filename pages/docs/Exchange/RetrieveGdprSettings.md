# Exchange
## Retrieve GDPR Settings
### SYNOPSIS
```
    Retrieves the Exchange GDPR related settings as a CSV string
```
### DESCRIPTION
```
    Retrieves the Exchange GDPR related settings as a CSV string.
    The settings retrieved are:
        Office 365 Message Encryption
            This performs a test of the Information Rights Management (IRM) configuration of the
            organization for functionality. Possible output values are 'Enabled' and 'Not Enabled'.
        Organization Data Location
            This retrieves the data locations for the various organizational units present.
        Advanced Threat Protection
            This retrieves whether Advanced Threat Protection is 'Enabled', 'Not Enabled', or
            'Not Available'.
        Connection Filtering Configuration
            This retrieves the connection filtering policies, and checks if they are the 'Default
            Configuration', a configured 'Advanced Configuration', or 'Not Configured'.
        Safe Sender Lists
            This performs a check of all the mailboxes and determines how many mailboxes have junk
            email configurations enabled, as well as how many mailboxes have junk email configurations
            actually configured.
        Spam Filter Policy
            This retrieves whether the spam filter policy is the 'Default Configuration' or an
            'Advanced Configuration'.
        Highest Bulk Email Threshold
            This retrieves all the bulk email thresholds among the hosted filter content policies,
            and outputs the highest threshold. The higher the bulk email threshold setting, the more
            bulk emails will be received.
        Device Security Policies
            This retrieves whether any device security policies are 'Configured', or if there are
            'No Configurations'.
        Default Data Loss Prevention Policy
            This retrieves whether the default Data Loss Prevention policy has been 'Enabled', or if
            it is 'Not Enabled'.
        Policy Tool Tips
            This retrieves whether policy tool tips are 'Enabled' or 'Not Enabled'.
        Policy Email Notifications
            This retrieves whether policy email notifications are 'Enabled' or 'Not Enabled'.
        Archive Mailboxes
            This retrieves the number of mailboxes for which archive has been enabled.
        Data Retention Policies
            This retrieves the various data retention policies, the tag links available
            within each policy, as well as the number of mailboxes using each policy.
        Litigation Holds
            This retrieves the number of mailboxes which have litigation hold active.
```
### INPUTS
```
    Office365AdministrativeCredentials
        A MSPComplete endpoint object containing the Office 365 administrative credentials.
```
### OUTPUTS
```
    ExchangeGdprSettingsCsv
        A CSV containing the retrieved settings. It consists of two columns: 'ComplianceItem' and
        'CurrentSetting'.
```
### NOTES
```
    Version: 1.1.0
    Last updated: 11 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

