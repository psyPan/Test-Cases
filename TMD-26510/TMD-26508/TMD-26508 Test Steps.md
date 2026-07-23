**Goal**
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

---
## Test Steps
1. Go To Models Library Page
2. open show hide column
3. **Verify The Auto Power Budget Fields Are Not Visible In Show/Hide Column Dialog Of Models Library**
4. Open Model `CoolingUnitModel26510`
5. Click `Power Supply Ports` Subtab
6. **Verify The Auto Power Budget Fields Are Not Visible In Model Detail**
    (TMD-17784     
    Items List::Open Item With Edit Mode    ${itemName}
    Item Detail::Wait Until Subtab Field Is Not Visible    ${dataCircuitCustomField17791.name}
    Items List::Close Tab    ${itemName}
    Items List::Click Clear Button)
7. Close Tab
8. Go To Items List Page
9.  Open Show/Hide Column  # show hide column 驗證,filter檢查有無支援class
10.  **Verify The Auto Power Budget Fields Are Not Visible In Show/Hide Column Dialog Of Items List**
11.  Open Item `COOLINGUNITITEM26510`
12. Click `Power Supply Ports` Subtab
13. **Verify The Auto Power Budget Fields Are Not Visible In Item Detail**