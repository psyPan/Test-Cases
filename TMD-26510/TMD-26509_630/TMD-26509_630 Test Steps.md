**Goal**
TMD-26509 Verify the Potential Power field in Cooling Unit Models
TMD-26630 Verify Fluid Flow Rate values in Cooling Unit.
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

### Power Supply Ports For Item `COOLINGUNITITEM26507`
- `Operation` : `ADD`
- `Object` : `POWER-PORT`
- `Item Location` : `SITE A`
- `Item Name` : `COOLINGUNITITEM26510`
- `Port Name` : `PS1`
- `Index` : `1`
- `Port Type` : `Power Supply`
- `Connector` : `IEC-320-C14`
- `Phase Type` : `Sinlge Phase (3-wire)`
- `Volt` : `120`
- `Power Factor` : `1`
- `Watts (N)` : `100`
- `Watts (B)` : `60`

- `Operation` : `ADD`
- `Object` : `POWER-PORT`
- `Item Location` : `SITE A`
- `Item Name` : `COOLINGUNITITEM26510`
- `Port Name` : `PS2`
- `Index` : `2`
- `Port Type` : `Power Supply`
- `Connector` : `IEC-320-C14`
- `Phase Type` : `Sinlge Phase (3-wire)`
- `Volt` : `120`
- `Power Factor` : `1`
- `Watts (N)` : `55`
- `Watts (B)` : `33`

## Test Steps
1. Create Power Supply Ports By File Import 
2. Go To Models Library Page
3. **Verify Value Of Potential Power Is Correct** (93)
4. Open Model `CoolingUnitModel26510` With Edit Mode
5. Click "Specification" Subtab
6. **Verify Empty Value For Fluid Flow Rate Is Valid**
7. Change Value Of "Fluid Flow Rate" To 8888888.8888
8. **Verify Validation Error Is Visible**
9. Change Value Of "Fluid Flow Rate" To 888888.88888
10. **Verify Validation Error Is Visible**
11. Change Value Of "Fluid Flow Rate" To -9
12. **Verify Validation Error Is Visible**
13. Change Value Of "Fluid Flow Rate" To 888888.8888
14. Save Model
15. Go To Items List Page
16. Open Item `COOLINGUNITITEM26510` With Edit Mode
17. Click "Configuration" Subtab
18. **Verify Values Of Fluid Flow Rate In Item Detail Is Same As Model's**
19. Change Value Of "Fluid Flow Rate" To 8888888.8888
20. **Verify Validation Error Is Visible**
21. Change Value Of "Fluid Flow Rate" To 888888.88888
22. **Verify Validation Error Is Visible**
23. Change Value Of "Fluid Flow Rate" To -9
24. **Verify Validation Error Is Visible**
25. Delete Value Of "Fluid Flow Rate"
26. Click Save Button
27. Change Value Of "Fluid Flow Rate" To 22
28. Click Save Button
29. Go To User Profile Page
30. Change Unit System To SI (Metric)
31. Click Save Button
32. Relogin To Items List Page
33. Open Item `COOLINGUNITITEM26510` With Edit Mode
34. Click "Configuration" Subtab
35. **Verify Unit And Value Of Fluid Flow Rate Display Convert To SI**