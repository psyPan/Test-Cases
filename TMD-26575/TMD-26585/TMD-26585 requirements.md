TMD-26585 Verify Heat Rejection import template contains required capacity and flow columns

## Test step
1. Download Models tempalte and select the Heat Rejection import sheet.
Verify the column headers include the following:
Compensation Factor
Nominal Capacity (Tons)
Nominal Capacity (kW)
Airflow Rate (cfm)
Fluid Flow Rate (gpm)

2. Use the template to import a Heat Rejection model with all fields filled with data
- after import, check the imported model

3. Export the imported model and make changes, then import again, Verify that chagnes you made are applied succsesfuly

## Test Result
The Heat Rejection import template contains the new columns. The user can import, export, and make changes and re-import the heat rejection models