## Test Case
TMD-26482 Age Derated Percentage Validation
TMD-26483 Age Derated Capacity Calculation

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

### Item
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HeatRejectionItem26477`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`

## Test Steps
1. Go to Items List Page
2. Open Item `HeatRejectionItem26477` With Edit Mode
3. Click Configuration Subtab
4. Change Age Derated % Value to -9
5. **Validation Error For Value < 0.1 Should Be Visible**
6. Repeat Step 4~5 With Value 0
7. Change Age Derated % Value to 100.01
8. **Validation Error For Value > 100 Should Be Visible**
9. Change Age Derated % Value To 100
10. Save Item
11. **Valid Value Should Be Visible**
12. Repeat Step 8~10 With Value 100.00
13. Change Age Derated % Value To 50
14. Save Item
15. **Verify Age Derated Capacity (Tons) Is Product Of Sensible Tons And Age Derated %**
16. **Verify Age Derated Capacity (kW) Is Product Of Sensible kW And Age Derated %**
17. **Verify Both Age Derated Capacity (Tons) And (kW) Fields Are Read Only**