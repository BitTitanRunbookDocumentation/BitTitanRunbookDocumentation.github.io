# Office 365
## Grant Public Folder Permissions
### SYNOPSIS
```
    Grant Public Folder Permissions
```
### DESCRIPTION
```
    Grant Public Folder Permissions to users.
    The users would be able to read, create, edit and delete items in the public folders, if they have the required permissions.
    The permissions include:
        ReadItems: The user has the right to read items within the specified public folder.
        CreateItems: The user has the right to create items within the specified public folder.
        EditOwnedItems: The user has the right to edit the items that the user owns in the specified public folder.
        DeleteOwnedItems: The user has the right to delete items that the user owns in the specified public folder.
        EditAllItems: The user has the right to edit all items in the specified public folder.
        DeleteAllItems: The user has the right to delete all items in the specified public folder.
        CreateSubfolders: The user has the right to create subfolders in the specified public folder.
        FolderOwner: The user is the owner of the specified public folder. The user has the right to view and move the public folder and create subfolders. The user can't read items, edit items, delete items, or create items.
        FolderContact: The user is the contact for the specified public folder.
        FolderVisible: The user can view the specified public folder, but can't read or edit items within the specified public folder.
    Permissions can be assigned based on the following roles:
        None: FolderVisible
        Owner: CreateItems, ReadItems, CreateSubfolders, FolderOwner, FolderContact, FolderVisible, EditOwnedItems, EditAllItems, DeleteOwnedItems, DeleteAllItems
        PublishingEditor: CreateItems, ReadItems, CreateSubfolders, FolderVisible, EditOwnedItems, EditAllItems, DeleteOwnedItems, DeleteAllItems
        Editor: CreateItems, ReadItems, FolderVisible, EditOwnedItems, EditAllItems, DeleteOwnedItems, DeleteAllItems
        PublishingAuthor: CreateItems, ReadItems, CreateSubfolders, FolderVisible, EditOwnedItems, DeleteOwnedItems
        Author: CreateItems, ReadItems, FolderVisible, EditOwnedItems, DeleteOwnedItems
        NonEditingAuthor: CreateItems, ReadItems, FolderVisible
        Reviewer: ReadItems, FolderVisible
        Contributor: CreateItems, FolderVisible
```
### INPUTS
```
    Usage option 1: Granting permissions for 1 user in 1 Public Folder
        PublicFolderIdentity
            A string representing the full path or name of the Public Folder, required
            Example: \Test\Directory\My Public Folder 1
            Example: Public Folder 1
        User
            Single MSPComplete end user that corresponds to the Office 365 user to grant the permissions, required
            If more than one object is provided, only the first one is used
        PublicFolderAccessRights
            A comma-delimited string representing the rights added to the user, required
            Example (Single Permission):    ReadItems
            Example (Multiple Permissions): ReadItems, CreateItems, DeleteOwnedItems, EditOwnedItems
            Example (Single Role):          Owner
            Example (Multiple Roles):       Reviewer, Contributor
    Usage option 2: Granting permissions for multiple users in Public Folders, using the inputs from a CSV file
        PublicFoldersCsv
            Required Columns:
                PublicFolderIdentity
                    A string representing the full path or name of the Public Folder
                User
                    The primary email address of the Office 365 user to grant the permissions
                PublicFolderAccessRights
                    A comma-delimited string representing the rights added to the user
```
### OUTPUTS
```
    ProcessedPublicFoldersCsv
        A CSV containing all the public folders which were processed by this task, as well as an additional
        column 'PublicFolderPermissionsGranted' to indicate if the permissions were granted successfully.
    Office365GrantPublicFolderPermissionsAllErrorMessages
        A string containing all the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0
    Last updated: 15 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

