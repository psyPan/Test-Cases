**Goal** not needed
TMD-26490 Heat Rejection Items Do Not Affect Cooling Zones
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
1. Get Number Of All Existing Cooling Zone Items, Get `Last Updated On` Value From All Existing Cooling Zone Items
2. Create Item `HEATREJECTIONITEM26477`
3. Get Number Of All Existing Cooling Zone Items, Get `Last Updated On` Value From All Existing Cooling Zone Items
4. **Verify Cooling Zone Items Are Not Created, Modified Or Deleted**
5. Delete Item `HEATREJECTIONITEM26477`
6. Get Number Of All Existing Cooling Zone Items, Get `Last Updated On` Value From All Existing Cooling Zone Items
7. **Verify Cooling Zone Items Are Not Created, Modified Or Deleted**