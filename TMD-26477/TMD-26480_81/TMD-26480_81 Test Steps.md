## Test Case
TMD-26480 Nominal Capacity fields are read-only
TMD-26481 Sensible Capacity values and Compensation Factor

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

1. `Class` : `HVAC`
2. `Subclass` : `Cooling Unit`
3. `Make` : `3Com`
4. `Model Name` : `CoolingUnitModel26480_81`
5. `Mounting` : `Rackable`
6. `Form Factor` : `Fixed`
7. `Height` : `1`
8. `Compensation Factor` : `50`
9. `Nominal Capacity (Tons)` : `100`

### Item
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HeatRejectionItem26477`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`

1. `Make` : `3Com`
2. `Model` : `CoolingUnitModel26480_81`
3. `Name` : `CoolingUnitItem26480_81`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`

## Test Steps
1. Go to Items List Page
2. Open Item `HeatRejectionItem26477` With Edit Mode
3. Click Configuration Subtab
4. **Nominal Capacity(tons) And Nominal Capacity(kW) Should Be Same As Model**
5. **Nominal Capacity(tons) And Nominal Capacity(kW) Should Be Read Only**
6. **Compensation Factor From Model Should Be Visible In % Column And Read-Only**
7. Change Sensible Capacity Tons Value to 123
8. Save item
9. **Sensible Capacity kW Value Should Be 432.57**
10. Repeat Test Steps From 1 to 8 For Item `CoolingUnitItem26480_81`