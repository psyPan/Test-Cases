**Goal**
TMD-26507 Verify the values of Effective Power and Potential Power fields for Cooling Unit
---
## Test Data
### Item
- `Make` : `APC`
- `Model` : `APC1000`
- `Name` : `COOLINGUNITITEM26507`
- `Status` : `Planned`
- `Location` : `Site A`

### Power Supply Ports For Item `COOLINGUNITITEM26507`
- `Operation` : `ADD`
- `Object` : `POWER-PORT`
- `Item Location` : `SITE A`
- `Item Name` : `COOLINGUNITITEM26507`
- `Port Name` : `PS1`, `PS2`, `PS3`, `PS4`, `PS5`
- `Index` : `1` ~ `5`
- `Port Type` : `Power Supply`
- `Connector` : `IEC-320-C14`
- `Phase Type` : `Sinlge Phase (3-wire)`
- `Volt` : `120~240`
- `Power Factor` : `1`
- `Watts (N)` : `55`
- `Watts (B)` : `33`

## Test Steps
1. Create Power Supply Ports By File Import 
2. Go To Item List Page
3. Open Item `COOLINGUNITITEM26507` With Edit Mode
4. Click "Power Supply Ports" Subtab
5. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=0, PP=132)
6. Change Second Port's "Connected Item" Status From Available To In Use
7. Click Save Button
8. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=33, PP=132)
9. Change Third Port's "Connected Item" Status From Available To In Use
10. Click Save Button
11. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=66, PP=132)
12. Change Third Port's "Connected Item" Status From In Use To Available
13. Click Connect Button
14. Click `Connect To VPC A`
15. Click Save Button
16. Go Back To `COOLINGUNITITEM26507` Item Detail
17. Click Refresh Button
18. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=66, PP=132)
19. Change Redundancy From `N+1` To `N`
20. Click Save Button
21. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=66, PP=165)
22. Close tab
23. Open Show/Hide Column
24. Select `Effective Power` and `Potential Power`
25. Click Apply Button
26. **Verify Values Of Effective Power And Potential Power In Items List Are Correct**(EP=66, PP=165)