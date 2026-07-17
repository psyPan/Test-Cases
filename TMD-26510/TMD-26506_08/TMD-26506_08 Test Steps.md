**Goal**
TMD-26506 Verify Potential Power and Effective Power fields for Cooling Unit
TMD-26508 Verify the auto power budget fields
---
## Test Data
### Models
#### Model
1. `Class` : `HVAC`
2. `Subclass` : `Cooling Unit`
3. `Make` : `3Com`
4. `Model Name` : `CoolingUnitModel26506_08`
5. `Mounting` : `Rackable`
6. `Form Factor` : `Fixed`
7. `Height` : `1`

### Item
#### Create Item
1. `Make` : `3Com`
2. `Model` : `CoolingUnitModel26506_08`
3. `Name` : `COOLINGUNITITEM26506_08`
4. `Status` : `Planned`
5. `Location` : `Site A`
6. `Cabinet` : `1A`
7. `U Position` : `Above`

### Power Supply Port
#### Create Power Supply Port
1. `Operation`: `ADD`
2. `Object`: `POWER-PORT`
3. `Item Location`: `SITE A`
4. `Item Name`: `COOLINGUNITITEM26506_08`
5. `Port Name`: `PS1`
6. `Port Type`: `Power Supply`
7. `Phase Type`: `Single Phase (3-Wire)`
8. `Volts`: `120`
9. `Power Factor`: `1`
10. `Watts (N)`: `100`
11. `Watts (B)`: `60`

---
## Test Steps
1. Create Power Supply Ports By File Import 
2. Go To Models Library Page
3. **Verify The Auto Power Budget Fields Are Not Visible In Models Library**
4. Open Model `CoolingUnitModel26506_08`
5. Click `Power Supply Ports` Subtab
6. **Verify The Auto Power Budget Fields Are Not Visible In Model Detail**
(TMD-17784     
Items List::Open Item With Edit Mode    ${itemName}
Item Detail::Wait Until Subtab Field Is Not Visible    ${dataCircuitCustomField17791.name}
Items List::Close Tab    ${itemName}
Items List::Click Clear Button)
7. Close Tab
8. Go To Items List Page
9. Open Show/Hide Column
10. Select `Potential Power ` And `Effective Power`
11. **Verify Potential Power and Effective Power Are Visible In Items List Page**
12. **Verify The Auto Power Budget Fields Are Not Visible In Items List Page**
13. Open Item `CoolingUnitItem26506_08`
14. Click `Power Supply Ports` Subtab
15. **Verify Potential Power and Effective Power Are Visible In Item Detail**
16. **Verify The Auto Power Budget Fields Are Not Visible In Item Detail**