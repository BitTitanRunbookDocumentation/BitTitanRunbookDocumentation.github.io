# Partner Center
## Suspend Customer Subscriptions
### SYNOPSIS
```
    Suspends Partner Center customer subscriptions as specified in a CSV string
```
### DESCRIPTION
```
    Suspends Partner Center customer subscriptions as specified in a CSV string
```
### INPUTS
```
    PartnerCenterAdministrativeCredentials
        A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
    CustomerSubscriptionsCsv
        A CSV string containing information about the subscriptions to be suspended, required.
        Required columns:
            Subscription
                A single string.
                This is the name of the subscription to suspend.
            Quantity
                A single string.
                This is the quantity of the subscription to suspend.
            Domain
                A single string.
                This is the domain of the customer for which the subscription will be suspended.
            OrderId
                A single string.
                This is the ID of the order which allocated this subscription to the customer.
```
### OUTPUTS
```
    UpdatedCustomerSubscriptionsCsv
        A CSV string containing the information about the subscriptions, as well as an additional column 'SuspendedSubscription' to indicate if the subscription was suspended.
    AllErrorMessages
        A string containing the error messages which were generated over the course of the task.
```
### NOTES
```
    Version: 1.1.2
    Last updated: 15 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

