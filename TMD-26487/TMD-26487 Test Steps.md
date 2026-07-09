**Goal**
TMD-26487 Fluid Flow Rate numeric validation
---
## Test Data
### Models
#### Model
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
#### Item
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HEATREJECTIONITEM26477`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`
---
## Test Steps
1. Go to Items List Page
2. Open Item `HeatRejectionItem26477` With Edit Mode
3. Open Configuration Subtab
4. Input `Fluid Flow Rate (gpm)` `9.99999`
5. **Verify Validation Error Is Visible**
6. Input `Fluid Flow Rate (gpm)` `9999999`
7. **Verify Validation Error Is Visible**
8. Input `Fluid Flow Rate (gpm)` `999999.9999`
9. Click Save Button
10. **Verify Valid Value Is Allowed**
11. Delete Value Of `Fluid Flow Rate (gpm)`
12. Click Save Button
13. **Verify Blank Value In "Fluid Flow Rate (gpm)" Is Allowed**

