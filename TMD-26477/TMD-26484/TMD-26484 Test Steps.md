## Test Case
TMD-26484 Airflow Rate Default and Validation
---
## Test Data
### Models
#### Model 1 -> With Airflow Rate
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

#### Model 2 -> Without Airflow Rate
1. `Class` : `HVAC`
2. `Subclass` : `Heat Rejection`
3. `Make` : `3Com`
4. `Model Name` : `HeatRejectionModel26484`
5. `Mounting` : `Rackable`
6. `Form Factor` : `Fixed`
7. `Height` : `1`

### Items
#### Item 1 -> Created From Model 1
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26477`
3. `Name` : `HEATREJECTIONITEM26477`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`

#### Item 2 -> Created From Model 2
1. `Make` : `3Com`
2. `Model` : `HeatRejectionModel26484`
3. `Name` : `HEATREJECTIONITEM26484`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`
---
## Test Steps
1. Open Item `HEATREJECTIONITEM26477` with edit mode
2. Click Configuration subtab
3. **Verify Airflow Rate (cfm) Field Has Same Value As Model**

4. Remove Airflow Rate (cfm)
5. Save Item
6. **Verify Item Without Airflow Rate (cfm) Can Be Saved** (The field is optional)
7. Close Item

8. Open Item `HEATREJECTIONITEM26484` with edit mode
9. Click Configuration subtab
10. **Verify Airflow Rate (cfm) Field Is Empty As Model**