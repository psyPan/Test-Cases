TMD-26442 Verfiy that if the column is not in the import sheet, it's value is assumed to be TRUE when add a new breaker via import
## Test Steps
1. Remove the "Derate Amps" column in the import template
2. Add the following breakers via import:
3. AC PANEL BREAKER (Local Panel/Remote Panel)

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
2. Check the value of the breakers on dcTrack

## Test Results
1. If the panel item's location country field is set United States
   1. The breakers can be added correctly
   2. The "Derate Amps" is assumed to be TRUE
2. If the panel item's location country field is set any other country
   1. The breakers can be added correctly
   2. The "Derate Amps" is assumed to be False