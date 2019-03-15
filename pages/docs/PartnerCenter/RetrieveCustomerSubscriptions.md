# Partner Center
## Retrieve Customer Subscriptions
### SYNOPSIS
```
    Retrieve Partner Center Customer Subscriptions as a CSV string.
```
### DESCRIPTION
```
    Retrieve Partner Center Customer Subscriptions as a CSV string.
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
    CustomerSubscriptionsCsv
        A CSV containing the following retrieved information about the customers' subscriptions:
            - The customer ID
            - The customer domain
            - The customer company name
            - The subscription name
            - The subscription quantity
            - The order ID of the subscription
            - Whether the subscription is an addon
```
### NOTES
```
    Version: 1.4.2
    Last updated: 15 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

