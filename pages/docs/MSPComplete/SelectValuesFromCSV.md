# MSPComplete
## Select Values From CSV
### SYNOPSIS
```
    Selects one or more values from a CSV string using the provided row indices and column names
```
### DESCRIPTION
```
    Selects one or more values from a CSV string using the provided row indices and column names.
    The values being returned are formatted as raw strings after extraction from the CSV, and subsequent
    post-processing of the value may be required to convert it to the desired output type.
    If the CSV is invalid, null strings are returned.
    If the row index or column name provided is invalid, a null string is also returned.
```
### INPUTS
```
    CsvString
        A string, required.
        The CSV string containing the values from which the intended values will be extracted.
    Selection1RowIndex
        A single string, required.
        This contains the string representation of the row index from which the first value will be
        extracted.
        The row indices start from 0 for the first row, 1 for the second row and so on.
    Selection1ColumnName
        A single string, required.
        This is the name of the column from which the first value will be extracted.
    Selection(X)RowIndex - Where (X) is 2, 3, 4, 5
        Same as Selection1RowIndex, optional.
        This is required if the corresponding Selection(X)ColumnName is specified.
    Selection(X)ColumnName
        Same as Selection1ColumnName, optional.
        This is required if the corresponding Selection(X)RowIndex is specified.
```
### OUTPUTS
```
    MSPCompleteSelectValueFromCsvSelectedValue(X) - Where (X) is 1, 2, 3, 4 and 5
        The various string values extracted from the CSV.
    MSPCompleteSelectValueFromCsvAllErrorMessages
        A string containing the error messages which were generated over the course of this task.
```
### NOTES
```
    Version: 1.1.0
    Last updated: 8 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

