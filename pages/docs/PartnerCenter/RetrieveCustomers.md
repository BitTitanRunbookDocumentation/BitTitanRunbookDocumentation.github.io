# Partner Center
## Retrieve Customers V2
### SYNOPSIS
```
    Retrieves Partner Center customers' information as a CSV string
```
### DESCRIPTION
```
    Retrieves Partner Center customers' information as a CSV string.
```
### INPUTS
```
    PartnerCenterAdministrativeCredentials
        A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
    CompanyNames
        One or more strings separated by a comma, optional.
        This specifies the company names for the customers which will be retrieved.
    Domains
        One or more strings separated by a comma, optional.
        This specifies the domains for the customers which will be retrieved.
```
### OUTPUTS
```
    CustomersCsv
        A CSV containing the following retrieved information about the customers:
            - The customer ID
            - The customer domain
            - The customer company name
```
### NOTES
```
    Version: 2.0.1
    Last updated: 3 October 2018
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

