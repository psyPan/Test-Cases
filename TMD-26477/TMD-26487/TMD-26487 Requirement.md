TMD-26487 Fluid Flow Rate numeric validation
## Test Steps
1. Enter a value with more than 2 decimal places
2. Enter a valid numeric value (10,2) # (10,4)
3. Leave the field blank

## Test Results
1. Validation error for more than 2 decimal places # 4
2. Valid numeric values are accepted
3. Blank value is allowed