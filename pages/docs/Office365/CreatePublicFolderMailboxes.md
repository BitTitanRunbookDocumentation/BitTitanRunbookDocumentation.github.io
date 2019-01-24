# Office 365
## Create Public Folder Mailboxes
### SYNOPSIS
```
    Create Public Folder Mailboxes
```
### DESCRIPTION
```
    Before a Public Folder can be created, at least 1 Public Folder Mailbox must be created.
    The task library component creates Public Folder Mailboxes from a list of mailbox names, using the New-Mailbox cmdlet.
    Public Folder Mailboxes are specially designed mailboxes that store the hierarchy and content of Public Folders.
    The first Public Folder Mailbox created in your Exchange organization is called the primary hierarchy mailbox.
    It contains the writeable copy of the hierarchy of Public Folders for the organization and Public Folder content.
    There can be only one writeable copy of the Public Folder hierarchy in your organization.
    All other Public Folder Mailboxes are called secondary Public Folder Mailboxes and contain a read-only copy of the hierarchy and the content for Public Folders.
```
### INPUTS
```
    PublicFolderMailboxNames is a list of Public Folder Mailbox names separated by newline. Example:
    Primary Hierarchy Mailbox
    Secondary Hierarchy Mailbox 01
    Secondary Hierarchy Mailbox 02
    Secondary Hierarchy Mailbox 03
```
### OUTPUTS
```
    AllErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0
    Last updated: 28 December 2018
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

