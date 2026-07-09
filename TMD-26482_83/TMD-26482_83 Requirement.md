TMD-26482 Age Derated Percentage Validation
## Test Steps
1. Open Configuration subtab
2. Enter Age Derated % less than 0.1
3. Enter Age Derated % greater than 100
4. Enter Age Derated % within valid range (0.1 – 100)

## Test Results
1. System displays validation error for values < 0.1
2. System displays validation error for values > 100
3. System accepts values between 0.1 and 100

TMD-26483 Age Derated Capacity Calculation
## Test Steps
1. Enter a valid Age Derated %
2. Observe Age Derated Capacity (Tons)
3. Observe Age Derated Capacity (kW)

## Test Results
1. Age Derated Capacity (Tons) = Sensible Tons × Age Derated %
2. Age Derated Capacity (kW) = Sensible kW × Age Derated %
3. Both fields are read-only