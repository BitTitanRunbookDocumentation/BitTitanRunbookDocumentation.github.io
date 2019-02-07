# MSPComplete
## Generate a Random Password
### SYNOPSIS
```
    Generates a random password with the given requirements
```
### DESCRIPTION
```
    Generates a random password with the given requirements. By default, the password will be
    8 characters long with a random number of lowercase, uppercase, digits and special
    characters.
```
### INPUTS
```
    NumberOfCharactersInPassword
        String, optional
        The length of the password, with a minimum length of 1
        Defaulted to 8 characters in password.
    MinimumNumberOfLowercaseCharacters
        String, optional
        The minimum number of lowercase characters in the password
        Set to -1 to indicate no lowercase characters should be present in the password
        Defaulted to 0, i.e. random number of lowercase characters
    MinimumNumberOfUppercaseCharacters
        String, optional
        The minimum number of uppercase characters in the password
        Set to -1 to indicate no uppercase characters should be present in the password
        Defaulted to 0, i.e. random number of uppercase characters
    MinimumNumberOfDigits
        String, optional
        The minimum number of numerical digits in the password
        Set to -1 to indicate no numerical digits should be present in the password
        Defaulted to 0, i.e. random number of digits
    MinimumNumberOfSpecialCharacters
        String, optional
        The minimum number of special characters in the password
        Set to -1 to indicate no special characters should be present in the password
        Defaulted to 0, i.e. random number of special characters
    SpecialCharactersToUse
        String, optional
        The special character set to use instead of the default special character set
```
### OUTPUTS
```
    NewPassword
        The randomly generated password
```
### NOTES
```
    Version: 1.3
    Last updated: 1 February 2019
    Copyright (c) BitTitan, Inc. All rights reserved.
    Licensed under the MIT License.
```

