**Goal**
TMD-26583 Verify Airflow Rate and Fluid Flow Rate labels/units update by Unit System and accept only values > 0 (including decimals for Fluid Flow Rate)

---
## Test Data
### Model
- `Class` : `HVAC`
- `Subclass` : `Heat Rejection`
- `Make` : `3Com`
- `Model Name` : `HeatRejectionModel26575`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

---
## Test Steps
1. Go To Models Library
2. Open model `HeatRejectionModel26575` with Edit Mode
3. **Verify Airflow Rate And Fluid Flow Rate Labels Display Correct Unit System For US Unit System**
   1. Verify Airflow Rate Label Displays "Airflow Rate (cfm)"
   2. Verify Fluid Flow Rate Label Displays "Fluid Flow Rate (gpm)"
4. **Verify Airflow Rate Accepts Value Greater Than Zero**
   1. Input Value 1 In Airflow Rate
   2. Verify Model Can Be Saved Successfully
5. **Verify Airflow Rate Rejects Value Smaller And Equal To Zero**
   1. Input Value 0 In Airflow Rate
   2. Verify Validation Error Is Displayed
   3. Save Button Is Disabled
   4. Input Value -1 In Airflow Rate
   5. Verify Validation Error Is Displayed
   6. Save Button Is Disabled
6. **Verify Fluid Flow Rate Field Is Optional**
   1. Input Value 1 In Fluid Flow Rate
   2. Save Model
   3. Input Empty Value In Fluid Flow Rate
   4. Save Model
   5. Fluid Flow Rate Value Should Be Empty
7. **Verify Fluid Flow Rate Accepts Greater Than Zero And Value With Two Decimals**
   1. Input Value 1 In Fluid Flow Rate
   2. Save Model
   3. Fluid Flow Rate Value Should Be 1
   4. Input Value 12.12 In Fluid Flow Rate
   5. Save Model
   6. Fluid Flow Rate Value Should Be 12.12
8. **Verify Fluid Flow Rate Field Enforces Value With Two Decimals**
   1. Input Value 12.345 In Fluid Flow Rate
   2. Save Model
   3. Fluid Flow Rate Value Should Be 12.34
9. **Verify Fluid Flow Rate Field Rejects Value Smaller And Equal To Zero**
   1. Input Value 0 In Fluid Flow Rate
   2. Verify Validation Error Is Displayed
   3. Save Button Is Disabled
   4. Input Value -5 In Fluid Flow Rate
   5. Verify Validation Error Is Displayed
   6. Save Button Is Disabled
10. Change Unit System To S.I.
11. Relogin To Models Library
12. Open Model `HeatRejectionModel26575` with Edit Mode
13. **Verify Airflow Rate And Fluid Flow Rate Labels Display Correct Unit System For S.I. Unit System**
   1. Verify Airflow Rate Label Displays "Airflow Rate (m3/h)"
   2. Verify Fluid Flow Rate Label Displays "Fluid Flow Rate (lpm)"
14. Repeat test steps 4.~9. For S.I. Unit System