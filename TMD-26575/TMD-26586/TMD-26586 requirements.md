TMD-26586 Verify Heat Rejection import adheres to Cooling Unit validations and UI validation rules; Fluid Flow Rate is optional

## Test step
1. Prepare a single Heat Rejection import file containing multiple items with the following scenarios:
-Item A: All fields valid, Fluid Flow Rate blank
-Item B: Fluid Flow Rate populated with a valid value (> 0, up to 2 decimals)
-Item C: Fluid Flow Rate = 0
-Item D: Fluid Flow Rate is negative (e.g., -1)
-Item E: Fluid Flow Rate has more than 2 decimals (e.g., 12.345)
-Item F: Invalid Compensation Factor (outside allowed range)
-Item G: Invalid Nominal Capacity (Tons)
-Item H: Invalid Nominal Capacity (kW)
-Item I: Invalid Airflow Rate (cfm) (≤ 0 or invalid format)

2. Import the prepared file in a single import run.

3. Review the import results for each item

## Test Result
Items A and B are imported successfully and models are created/updated correctly.

Item A: Blank Fluid Flow Rate is accepted.

Item B: Fluid Flow Rate value is saved correctly with up to 2 decimal places.

Items C and D: Import fails with validation errors indicating values must be greater than 0.

Item E: Import enforces numeric(10,2) behavior (rejected or rounded/truncated in line with UI rules).

Items F–I: Each item fails with the same validation behavior and error messages as:

Cooling Unit import validations, and

Corresponding UI validations.

Invalid items do not create or update models.

Import results clearly display item-level validation errors.