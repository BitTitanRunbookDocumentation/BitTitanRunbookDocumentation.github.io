# Office 365
## Send Email V2
### SYNOPSIS
```
    Sends an email from an Office 365 mailbox with attachments
```
### DESCRIPTION
```
    Sends an email from an Office 365 mailbox with attachments
    If the attachments are in text format (i.e. extension with txt, csv, log, bat, dat), no encoding
    of the attachment contents is required.
    Otherwise if the attachments are not in text format, the attachment file bytes are to be encoded
    in Base64.
```
### INPUTS
```
    Office365EmailCredentials
        A MSPComplete endpoint object containing the Office 365 email credentials, required.
    EmailToAddress
        One or more strings separated by a newline, required.
        These are the destination email addresses for the email.
    EmailSubject
        A single string, required.
        This is the subject line of the email.
    EmailBody
        A single string, required.
        This is the main content of the email.
    EmailCcAddress
        One or more strings separated by a newline, optional.
        These are the email addresses which will receive carbon copies of the email.
    EmailBccAddress
        One or more strings separated by a newline, optional.
        These are the email addresses which will receive blind carbon copies of the email.
    Attachment1FileName
        A single string, in the format of FILENAME.EXTENSION, optional.
        Examples: report.pdf
    Attachment1FileContents
        A single string, optional.
        If the attachment is in text format, this should be the text contents of the attachment.
        If the attachment is in non-text format, this should be the Base64 encoded byte contents
        of the attachment file, using
        [Convert]::ToBase64String((Get-Content -Encoding Byte -Path FILE_PATH)).
    Attachment(X)FileName - Where (X) is 2, 3, 4 or 5
        Same as Attachment1FileName, optional
    Attachment(x)FileContents - Where (X) is 2, 3, 4 or 5
        Same as Attachment1FileContents, optional
```
### OUTPUTS
```
    None
```
### NOTES
```
    Version: 2.2.0
    Last updated: 1 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

