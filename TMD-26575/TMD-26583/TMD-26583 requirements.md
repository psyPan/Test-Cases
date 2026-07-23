TMD-26583 Verify Airflow Rate and Fluid Flow Rate labels/units update by Unit System and accept only values > 0 (including decimals for Fluid Flow Rate)

## Test step
1. Set Unit System = US in User Preference settings and verify that:
- Airflow Rate unit displays as cfm.
- Fluid Flow Rate label displays as Fluid Flow Rate (gpm).

2. Set Unit System = SI (Metric) in User Preference settings and refresh/reopen the model, verify that:
-Airflow Rate unit displays as m3/h.
-Fluid Flow Rate label displays as Fluid Flow Rate (lpm).

3. In the current Unit System, enter a valid value > 0 in Airflow Rate (e.g., 1) and save, verify that:
-Value is accepted and saved successfully, and there are no validation errors

4. Enter 0 in Airflow Rate and attempt to save and verify that:
- Validation error is displayed, and save is blocked.
- Enter -1 in Airflow Rate, and validate that the user is not able to save the model, and a validation error appears

5. Verify the Fluid Flow Rate field is optional by leaving it blank and saving.
~~Model saves successfully, and no required~~ field error is shown.

6. Enter a value > 0 with up to 2 decimals in Fluid Flow Rate (e.g., 12.34) and save.
- Value is accepted and saved successfully.
- Stored/displayed value keeps up to 2 decimals.
- Enter a value with more than 2 decimals (e.g., 12.345) and attempt to save and verify that the system enforces numeric(10,3) behavior
-Enter 0 in Fluid Flow Rate and attempt to save, then verify that a validation error is displayed and the save is blocked.
-Enter a negative value (e.g., -5) in Fluid Flow Rate and attempt to save and verify that: Validation error is displayed, and the save is blocked.

## Test Result
Units/labels switch correctly based on Unit System:
- Airflow: cfm (US), m3/h (SI)
- Fluid Flow: (gpm) (US), (lpm) (SI)

Airflow Rate accepts only values > 0.

Fluid Flow Rate is optional, accepts > 0, supports up to 2 decimals (numeric(10,2)).

Invalid values block save with clear validation messaging.