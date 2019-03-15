# Partner Center
## Allocate Subscriptions to Customers
### SYNOPSIS
```
    Allocates subscriptions to Partner Center Customers as specified in a CSV string
```
### DESCRIPTION
```
    Allocates subscriptions to Partner Center Customers as specified in a CSV string.
    This task does not check to see if the customer is currently already allocated the subscriptions.
    Running this task for a customer with existing subscriptions may result in the customer having extra unused subscriptions.
```
### INPUTS
```
    PartnerCenterAdministrativeCredentials
        A MSPComplete endpoint object containing the Partner Center administrative credentials, required.
    CustomerSubscriptionsCsv
        A CSV string containing information about the subscriptions which will be allocated to the customer.
        Required columns:
            Subscription
                A single string.
                This is the name of the subscription which will be allocated.
            Quantity
                A single string.
                This is the quantity of the subscription which will be allocated.
        Optional columns:
            Domain
                A single string. Either this or CustomerId must be provided.
                This is the domain of the company which will receive the subscription.
            CustomerId
                A single string. Either this or Domain must be provided.
                This is the customer ID of the company which will receive the subscription.
```
### OUTPUTS
```
    UpdatedCustomerSubscriptionsCsv
        A CSV string containing the information about the subscriptions which were allocated to the customer, as well as an additional column 'AllocatedSubscription' to indicate if the allocation succeeded.
        If the allocation succeeded, it will contain an 'OrderId' column to indicate the ID of the order used to allocate the subscription.
    AllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.3.1
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

