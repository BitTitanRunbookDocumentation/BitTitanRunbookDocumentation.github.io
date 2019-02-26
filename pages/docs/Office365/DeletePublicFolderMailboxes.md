# Office 365
## Delete Public Folder Mailboxes
### SYNOPSIS
```
    Delete Public Folder Mailboxes
```
### DESCRIPTION
```
    The task library component deletes Public Folder Mailboxes from a list of mailbox names, using the Remove-Mailbox cmdlet.
    Public Folder Mailboxes are specially designed mailboxes that store the hierarchy and content of Public Folders.
    At least 1 Public Folder Mailbox must be present in the organization, before a Public Folder can be created.
```
### INPUTS
```
    PublicFolderMailboxNames is a list of Public Folder Mailbox names separated by newline. Example:
    Secondary Hierarchy Mailbox 01
    Secondary Hierarchy Mailbox 02
    Secondary Hierarchy Mailbox 03
```
### OUTPUTS
```
    Office365DeletePublicFolderMailboxesErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1
    Last updated: 22 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

