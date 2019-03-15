# Partner Center
## Add Subscription to Customer V2
### SYNOPSIS
```
    Adds a subscription to a Partner Center customer.
```
### DESCRIPTION
```
    Adds a subscription to a Partner Center customer.
```
### INPUTS
```
    PartnerCenterAdministrativeCredentials
        A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
    SubscriptionName
        A single string, required.
        This is the name of the subscription which will be allocated to the customer.
    Quantity
        A single string, required.
        This is the quantity of the subscription which will be allocated to the customer.
    Domain
        A single string, optional. Either this or CustomerId must be provided.
        This is the domain of the company which will receive the subscription.
    CustomerId
        A single string, optional Either this or Domain must be provided.
        This is the customer ID of the company which will receive the subscription.
```
### OUTPUTS
```
    None
```
### NOTES
```
    Version: 2.0.0
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

