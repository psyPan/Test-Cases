**Goal**
TMD-26485 Fluid Flow Rate field label changes based on Unit System
TMD-26488 Fluid Flow Rate column visibility in Item List
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
(Tag) -> Single Process Only
1. Open Item `HEATREJECTIONITEM26477` With Edit Mode
2. Open Configuration Subtab
3. **Verify Fluid Flow Rate Label displays “Fluid Flow Rate (gpm)”**
4. Input Value `Fluid Flow Rate (gpm)`: `100`
5. Save and Close Item
6. **Verify "Fluid Flow Rate" Column Is Not Visible In Items List Page**
7. Open Show/Hide Column
8. Select "Fluid Flow Rate" In Show/Hide Column And Click Apply
9. **Verify “Fluid Flow Rate” Column Value In Items List Page Is Same As In Item Detail**
10. Open Show/Hide Column
11. Unselect "Fluid Flow Rate" In Show/Hide Column And Click Apply
12. **Verify "Fluid Flow Rate" Column Is Not Visible In Items List Page**
13. Go To User Profile Page
14. Change Unit System to SI (Metric)
15. Relogin To Items List page
16. Open Item `HEATREJECTIONITEM26477` With View Mode And Open Configuration Subtab
17. **Verify Fluid Flow Rate Label displays “Fluid Flow Rate (lpm)”**
18. **Verify “Fluid Flow Rate (lpm)” Value Changes When Unit System Is Changed**
19. Close Item
20. Open Show/Hide Column In Item List
21. Select "Fluid Flow Rate" In Show/Hide Column And Click Apply
22. **Verify “Fluid Flow Rate” Column Value In Items List Page Is Same As In Item Detail**
23. Repeat steps 13~16 to change unit system back to US
24. **Verify US Value Of Fluid Flow Rate Is Same When Changing Back To US Unit System** (`Fluid Flow Rate (gpm)`: `100`)
25. Close Item And Clear Filter In Items List page