# Partner Center
## Remove Reseller Relationship
### SYNOPSIS
```
    Removes the Partner Center Reseller Relationship with one or more Partner Center customers
```
### DESCRIPTION
```
    Removes the Partner Center Reseller Relationship with one or more Partner Center customers
```
### INPUTS
```
    PartnerCenterAdministrativeCredentials
        A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
    CustomersCsv
        A CSV string containing the information about the customers which will be removed.
        Optional columns:
            Domain
                A single string. Either this or CustomerId must be provided.
                This is the domain of the company which will be removed.
            CustomerId
                A single string. Either this or Domain must be provided.
                This is the customer ID of the company which will be removed.
```
### OUTPUTS
```
    UpdatedCustomersCsv
        A CSV string containing the information about the customers, as well as an additional column 'RemovedResellerRelationship' to indicate if the removal of the relationship was successful.
    AllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.2.3
    Last updated: 15 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

