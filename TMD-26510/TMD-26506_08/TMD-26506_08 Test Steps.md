**Goal**
TMD-26506 Verify Potential Power and Effective Power fields for Cooling Unit
TMD-26508 Verify the auto power budget fields
---
## Test Data
### Model
- `Class` : `HVAC`
- `Subclass` : `Cooling Unit`
- `Make` : `3Com`
- `Model Name` : `CoolingUnitModel26510`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

### Item
- `Make` : `3Com`
- `Model` : `CoolingUnitModel26510`
- `Name` : `COOLINGUNITITEM26510`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

### Power Supply Port
- `Operation`: `ADD`
- `Object`: `POWER-PORT`
- `Item Location`: `SITE A`
- `Item Name`: `COOLINGUNITITEM26510`
- `Port Name`: `PS1`
- `Port Type`: `Power Supply`
- `Phase Type`: `Single Phase (3-Wire)`
- `Volts`: `120`
- `Power Factor`: `1`
- `Watts (N)`: `100`
- `Watts (B)`: `60`

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