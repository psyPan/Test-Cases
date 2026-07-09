TMD-26480 Nominal Capacity fields are read-only
## Test Steps
1. Open Heat Rejection item Configuration subtab
2. Attempt to edit both values Nominal Capacity (Tons) and Nominal Capacity (kW)

## Test Results
1. Verify Nominal Capacity (Tons) displays model value and is read-only populated from the model
2. Verify Nominal Capacity (kW) displays model value and is read-only populated from the model
3. Verify Editing is not allowed

TMD-26481 Sensible Capacity values and Compensation Factor
## Test Steps
1. Open Configuration subtab
2. Verify % column value for sensible row
3. Edit Sensible Capacity (Tons)
4. Edit Sensible Capacity (kW)

## Test Results
1. Verify % column displays Compensation Factor (%) from model and it's read-only
2. Verify Sensible Capacity Tons and kW fields are editable, both are updated if you change one of them. Cooling unit has the same behavior