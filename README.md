# Password Validator

A simple password validation library that ensures passwords meet specific security requirements.

## Requirements

The password validator checks that passwords meet the following criteria:
- Minimum length of 8 characters
- Must start with a letter
- Must contain at least one capital letter
- Must contain at least one lowercase letter
- Must contain at least one number
- Must contain an underscore (_)

## Project Structure

```
tdd_sample/
├── PasswordValidator.cs    # Main validator implementation
├── ValidatorTests.cs      # xUnit test cases
└── README.md             # This file
```

## Running Tests

The project uses xUnit for testing. To run the tests:

1. Make sure you have .NET SDK installed
2. Navigate to the project directory
3. Run: `dotnet test`

## Test Cases

The following test cases are implemented:
- Too short password
- Missing capital letter
- Missing lowercase letter
- Missing number
- Missing underscore
- Starting with number
- Valid password

## Example Usage

```csharp
var validator = new PasswordValidator();
bool isValid = validator.Validate("Password_123"); // Returns true
```
