## Test Case
TMD-26478 Configuration subtab for Heat Rejection
TMD-26479 Fields in Configuration subtab

## Test Data
### Model
1. `Class` : `HVAC`
2. `Subclass` : `Heat Rejection`
3. `Make` : `3Com`
4. `Model Name` : `HeatRejectionModel26477`
5. `Mounting` : `Rackable`
6. `Form Factor` : `Fixed`
7. `Height` : `1`
8. `Nominal Capacity (Tons)` : `100`

### Item
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HEATREJECTIONITEM26477`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`

## Test Steps
1. Go to Items List Page
2. Open Item `HeatRejectionItem26477` With Edit Mode
3. **Configuration Subtab Should Be Visible**
4. Click Configuration Subtab
5. **Nominal, Sensible, Age Derated Rows Should Be Visible**
6. **Airflow Rate And FluidFlow Rate Should Be Visible**