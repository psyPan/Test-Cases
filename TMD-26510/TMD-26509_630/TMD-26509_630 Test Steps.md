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

### Power Supply Ports For Model `CoolingUnitModel26510`
- `Operation` : `ADD`
- `Object` : `POWER-PORT`
- `Model Name` : `CoolingUnitModel26510`
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
- `Moel Name` : `CoolingUnitModel26510`
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
1. Create Power Supply Ports In Model by file import
2. Go To Models Library Page
3. **Verify Value Of Potential Power Is Correct** (120)
4. Open Model `CoolingUnitModel26510` With Edit Mode
5. Click "Specification" Subtab
6. **Verify it has a field Fluid Flow Rate which is below the Airflow Rate in the Configuration sub-tab**
7. Change Value Of "Fluid Flow Rate" To 888888.8888
8. Click Save Button
9. Change Value Of "Fluid Flow Rate" To empty
10. Click Save Button
11. **Verify Empty Value For Fluid Flow Rate Is Valid**
12. Change Value Of "Fluid Flow Rate" To 8888888.8888
13. **Verify Validation Error Is Visible**
14. Change Value Of "Fluid Flow Rate" To 888888.88888
15. **Verify Validation Error Is Visible**
16. Change Value Of "Fluid Flow Rate" To -9
17. **Verify Validation Error Is Visible**
18. Change Value Of "Fluid Flow Rate" To 888888.8888
19. Click Save Button
20. Go To Items List Page
21. Open Item `COOLINGUNITITEM26510` With Edit Mode
22. Click "Configuration" Subtab
23. **Verify Values Of Fluid Flow Rate In Item Detail Is Same As Model's**
24. Delete Value Of "Fluid Flow Rate"
25. Click Save Button
26. **Verify Empty Value For Fluid Flow Rate Is Valid**
27. Change Value Of "Fluid Flow Rate" To 8888888.8888
28. **Verify Validation Error Is Visible**
29. Change Value Of "Fluid Flow Rate" To 888888.88888
30. **Verify Validation Error Is Visible**
31. Change Value Of "Fluid Flow Rate" To -9
32. **Verify Validation Error Is Visible**
33. Change Value Of "Fluid Flow Rate" To 22
34. Click Save Button
35. Go To User Profile Page
36. Change Unit System To SI (Metric)
37. Click Save Button
38. Relogin To Items List Page
39. Open Item `COOLINGUNITITEM26510` With View Mode
40. Click "Configuration" Subtab
41. **Verify Unit And Value Of Fluid Flow Rate Display Convert To SI**