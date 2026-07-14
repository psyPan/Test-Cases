**Goal**
TMD-26492 Import Validation Rules
---
## Test Data
### Model
1. `Class` : `HVAC`
2. `Subclass` : `Heat Rejection`
3. `Make` : `3Com`
4. `Model Name` : `HeatRejectionModel26477`
5. `Mounting` : `Rackable`
6. `Form Factor` : `Fixed`
7. `Height` : `1`
8. `Compensation Factor` : `50`
9. `Nominal Capacity (Tons)` : `100`
10. `Airflow Rate (cfm)` : `100`

### Items
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HEATREJECTIONITEM26492-1`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`
8. `Sensible Capacity (Tons)` : `50`
9. `Airflow Rate (cfm)` : `50`

1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HEATREJECTIONITEM26492-2`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`
8. `Sensible Capacity (Tons)` : `-9`
9. `Airflow Rate (cfm)` : `-100`
10. `Fluid Flow Rate (gpm)` : `8888888.8888`

1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HEATREJECTIONITEM26492-3`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`
8. `Sensible Capacity (Tons)` : `50`
9. `Airflow Rate (cfm)` : `50`
10. `Fluid Flow Rate (gpm)` : `888888.88888`
---
## Test Steps
1. Go To File Import Page
2. Create Item By File Import
3. **Verify Error Message Is Visible For Invalid Sensible Capacity, Airflow Rate And Fluid Flow Rate Format**
4. Go To Items List Page
5. **Verify Item Without Fluid Flow Rate Value Is Created**