TMD-26445 Verify the new column is implemented for the Add operations
## Test Steps
1. ADD the following breakers via import with the value of "Derate Amps" column set to TRUE/FALSE :
2. AC PANEL BREAKER (Local Panel/Remote Panel)

Assignment type:
- 
   - BREAKER TO CABINET
   - BREAKER TO POSITION
   - BREAKER TO ROW
   - BREAKER TO PANEL
   - BREAKER TO SPACE
   - BREAKER TO OTHER
- BUSWAY BREAKER
- DC PANEL BREAKER (Plant Panel/DC Panel)

Assignemt Type:
1. 
   - BREAKER TO CABINET DC
   - BREAKER TO SPACE DC
   - BREAKER TO OTHER DC
2. Check the result

## Test Results
1. The breakers can be added correctly
2. The "Derate Amps" is set to TRUE/FALSE accordingly