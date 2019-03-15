# Excel
## Set Cell Values
### SYNOPSIS
```
    Sets the values of cells in an Excel workbook
```
### DESCRIPTION
```
    Sets the values of cells in an Excel workbook.
    Given an Base64 encoded Excel workbook, this task can set the value in a range of cells for a worksheet from specified inputs or can set values in a range of cells for multiple worksheets via CSV input.
    The output will be the updated Excel workbook bytes encoded in Base64.
```
### INPUTS
```
    Usage option 1: Set the value of the specified cells on a worksheet
        ExcelWorkbookBase64EncodedBytes
            Single string, required
            The Excel worksheet which has been encoded in Base64
        Cells
            Single string describing the cell/range of cells to update, required
        Value
            Single string, required
        Worksheet
            Single string, required
            The name of the worksheet to set the cell values
    Usage option 2: For each row in the csv file, set the value of the specified cells on a worksheet
        ExcelWorkbookBase64EncodedBytes
            Single string, required
            The Excel worksheet which has been encoded in Base64
        CellValuesCsv
            Required columns:
                Cells
                    String describing the cell/range of cells to update
                Value
                    The value to set in the cells
                Worksheet
                    The name of the worksheet to set the cell values
```
### OUTPUTS
```
    ProcessedExcelWorkbookBase64EncodedBytes
        Base64 encoded bytes
        The updated (processed) Excel workbook
        To convert back to an Excel file, use [Convert]::FromBase64String($ExcelWorkbookBase64EncodedBytes) | Set-Content -Encoding Byte -Path FILE_PATH
    ExcelSetCellValuesCsv
        String, CSV format
        The CellValuesCsv with additional column 'SetSuccessfully' to indicate if the operation has occurred successfully or not
    ExcelSetCellValuesErrorMessages
        String
        A string containing all the error messages which were generated over the course of this task
```
### NOTES
```
    Version: 1.0.2
    Last updated: 14 March 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

