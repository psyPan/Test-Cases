TMD-26577 Verify validation, boundaries, and warning behavior for Compensation Factor (%) field

## Test step
1. Locate the Compensation Factor (%) field on the Specification subtab.
2. Verify that the field is marked as required.
3. Check boundary values by entering the following values one at a time and attempting to save:
-1 (minimum valid value)
-200 (maximum valid value)
-0 (below minimum)
-201 (above maximum)
4. Verify that appropriate validation errors appear for invalid values.
5. Enter a value greater than 100 and less than or equal to 200 (e.g., 120).
6. Observe the field behavior after entering the value.

## Test Result
The Compensation Factor (%) field is displayed and marked as required.

The system accepts values greater than or equal to 1 and less than or equal to 200.

Entering values below 1 or above 200:
-Displays a validation error.
-Prevents saving the model.

When a value greater than 100 is entered: - A warning icon appears next to the field.
The warning does not block saving the model.

No warning is displayed for values 100 or less.