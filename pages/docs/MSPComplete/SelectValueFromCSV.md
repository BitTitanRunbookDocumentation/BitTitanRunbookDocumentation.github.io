# MSPComplete
## Select Value From CSV
### SYNOPSIS
```
    Selects a single value from a CSV string using the provided row index and column name
```
### DESCRIPTION
```
    Selects a single value from a CSV string using the provided row index and column name.
    The value being returned is formatted as a raw string after extraction from the CSV, and post-
    processing of the value may be required to convert it to the desired type.
    If the CSV is invalid, a null string is returned.
    If either the row index and/or column name provided are invalid, a null string is returned.
```
### INPUTS
```
    CsvString
        String, required.
        The CSV string containing the values from which the intended value will be extracted.
    RowIndex
        Single string, required.
        This contains the string representation of the row index from which the value will be extracted.
        The row indices start from 0 for the first row, 1 for the second row and so on.
    ColumnName
        Single string, required.
        The name of the column
```
### OUTPUTS
```
    MSPCompleteSelectValueFromCsvSelectedValue
        The string value extracted from the CSV.
    MSPCompleteSelectValueFromCsvAllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.0
    Last updated: 22 January 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

