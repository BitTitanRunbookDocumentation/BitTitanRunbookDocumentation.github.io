# Active Directory
## Update Users' Attributes
### SYNOPSIS
```
    Updates attributes within users in Active Directory
```
### DESCRIPTION
```
    Updates attributes within users in Active Directory.
    This task is able to:
        Add values to existing user attributes
        Clear existing user attribute values
        Remove values from user attributes
        Replace the existing set of user attribute values with new values
```
### INPUTS
```
    Usage option 1: Update an attribute within a user
        User
            A single MSPComplete end user object, required.
            This is the user in Active Directory which will receive the attribute update.
            The user object is required have an 'OnPremisesSecurityIdentifier' extended property, which corresponds to the 'objectSID' or 'SID' property on the Active Directory user.
        AttributeName
            A single string, required.
            This specifies the name of the attribute to be updated within the user.
        AttributeValues
            One or more strings separated by a newline, required.
            This specifies the values which are used to update the user attribute.
            This is optional if the value for Action is 'Clear'.
        Action
            A single string, required.
            Valid values are 'Add', 'Clear', 'Remove' and 'Replace'.
            Add: Adds the values specified in AttributeValues to the existing attribute values
            Clear: Clears the existing attribute values
            Remove: Removes the values specified in AttributeValues from the existing attribute values
            Replace: Replaces the existing attribute values with the values specified in AttributeValues
    Usage option 2: Update attributes within users via CSV
        AttributesCsv
            Required columns:
                UserIdentity
                    A single string, required.
                    This identifies the user in Active Directory. The identity can be
                        - A distinguished name
                        - A GUID (objectGUID)
                        - A security identifier (objectSid)
                        - A SAM account name (sAMAccountName)
                AttributeName
                    A single string, required.
                    This specifies the name of the attribute to be updated within the user.
                AttributeValues
                    One or more strings separated by a comma and enclosed in double quotes, required.
                    Example: "value1,value2"
                    This specifies the values which are used to update the user attribute.
                    This is optional if the value for Action is 'Clear'.
                Action
                    A single string, required.
                    Valid values are 'Add', 'Clear', 'Remove' and 'Replace'.
                    Add: Adds the values specified in AttributeValues to the existing attribute values
                    Clear: Clears the existing attribute values
                    Remove: Removes the values specified in AttributeValues from the existing attribute values
                    Replace: Replaces the existing attribute values with the values specified in AttributeValues
```
### OUTPUTS
```
    ActiveDirectoryUpdateUsersAttributesCsv
        A CSV string containing information about the user attributes which were updated, as well as an additional column 'AttributeUpdated' to indicate if the attribute was updated successfully.
    ActiveDirectoryUpdateUsersAttributesErrorMessages
        A string containing all the errors messages which were generated over the course of this task.
```
### NOTES
```
    Version: 2.0.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

