TMD-26492 Import Validation Rules
## Test Steps
1. Create import file with invalid values
2. Import file without Fluid Flow Rate
3. Import file with invalid Fluid Flow Rate format

## Test Results
1. Import fails with validation errors for invalid data
2. Import succeeds when Fluid Flow Rate is missing
3. Import fails for invalid Fluid Flow Rate format