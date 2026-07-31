TMD-26444 Verfiy that an error will be generated if the value of the "Derate Amps" column in the import sheet is blank or non-boolean
## Test Steps
1. ADD/EDIT the following breakers via import with the value of "Derate Amps" column set to blank :
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

---
1. ADD/EDIT the following breakers via import with the value of "Derate Amps" column set to non-boolean (E.g., set to numeric) :
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
1. The import should fail and that row will generate an error. "Line xxx - Derate Amps column must contain the value TRUE or FALSE"
---
1. The import should fail and that row will generate an error. "Line xxx - Derate Amps column must contain the value TRUE or FALSE"