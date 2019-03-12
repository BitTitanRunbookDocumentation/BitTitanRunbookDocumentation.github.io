# Office 365
## Block All Incoming Mail from Domain
### SYNOPSIS
```
    Create and apply rule to block all incoming mail into Office 365 that originates from
    specified domains, replying with a rejection message if provided
```
### DESCRIPTION
```
    Creates and applies a rule to block all incoming mail into Office 365 that originates from the
    specified domains, replying with a rejection message if provided.
    This block is applied organization-wide.
    If the mail rejection message is not provided, the mail will be blocked silently.
```
### INPUT
```
    Usage option 1: Create and apply a mail block rule against the specified domains
        Office365AdministrativeCredentials
            A MSPComplete endpoint object containing the Office 365 administrative credentials, required.
        Domain
            String, required
            The list of domains (separated by a comma) to block incoming mail from
        BlockRuleName
            String, optional
            The name for the block rule. if no name is provided, will default to
            'Block all incoming mail from x, y, z' (where x, y, z is the domains supplied)
        MailRejectMessage
            String, optional
            The rejection message back to the sender. If no rejection message is supplied, the mail
            will be blocked silently
```
### OUTPUT
```
    None
```
### NOTES
```
    Version: 1.0
    Last updated: 11 October 2018
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

