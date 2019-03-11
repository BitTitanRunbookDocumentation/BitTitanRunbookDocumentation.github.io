# MSPComplete
## Transpose CSVs
### SYNOPSIS
```
    Transposes CSV data
```
### DESCRIPTION
```
    Transposes CSV data for up to five CSV strings.
    The CSV string header will be transposed into a "Name" column.
    If there is only one data row in the CSV string, it will be transposed into a "Value" column.
    If there is more than one data row in the CSV string, they will be transposed into "Value1",
    "Value2", "Value3" etc., columns.
```
### INPUTS
```
    Csv1
        A single string, required.
    Csv(X) - Where (X) is 2, 3, 4, 5
        Same as Csv1, optional
```
### OUTPUTS
```
    TransposedCsv(X) - Where (X) is 1, 2, 3, 4, 5
        This is the result of transposing each of the CSV strings.
    MSPCompleteTransposeCsvsErrorMessages
        A string containing the error messages generated over the course of this task.
```
### NOTES
```
    Version: 1.0.0
    Last updated: 11 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

