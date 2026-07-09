TMD-26485 Fluid Flow Rate field label changes based on Unit System
## Test Steps
1. Set Unit System to US
2. Open Heat Rejection item Configuration subtab
3. Verify Fluid Flow Rate label
4. Change Unit System to SI (Metric)
5. Reopen Configuration subtab

## Test Results
1. Verify label displays “Fluid Flow Rate (gpm)” for US
2. Verify label displays “Fluid Flow Rate (lpm)” for SI
3. Verify item list label is updated (issue, DCT-82134)
4. Verify values are updated -> Recheck Fluid Flow Rate (gpm) is the same after changing back from SI to US

TMD-26488 Fluid Flow Rate column visibility in Item List
## Test Steps
1. Open Item List
2. Open Show/Hide Columns settings
3. Enable Fluid Flow Rate column
4. Disable Fluid Flow Rate column

## Test Results
1. Fluid Flow Rate column is hidden by default
2. Column appears when enabled
3. Column hides again when disabled