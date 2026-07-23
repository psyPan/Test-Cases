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
- `Item Name` : `COOLINGUNITITEM26507`
- `Port Name` : `PS1`, `PS2`, `PS3`, `PS4`, `PS5`
- `Connector` : `IEC-320-C14`
- `Phase Type` : `Sinlge Phase (3-wire)`
- `Volt` : `120~240`
- `Power Factor` : `1`
- `Watts (N)` : `55`
- `Watts (B)` : `33`

## Test Steps
1. Go To Item List Page
2. Open Item `COOLINGUNITITEM26507` With Edit Mode
3. Click "Power Supply Ports" Subtab
4. Input `Quantity` : `1`
5. Input `Connector` : `IEC-320-C14`
6. Input `Watts (N)` : `55`
7. Input `Quantity` : `5`
8. Input `Redundancy` : `N+1`
9. Click Save Button
10. **Verify Potential Power and Effective Power Are Visible In Item Detail**
11. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=0, PP=132)
12. Change Second Port's "Connected Item" Status From Available To In Use
13. Click Save Button
14. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=33, PP=132)
15. Change Third Port's "Connected Item" Status From Available To In Use
16. Click Save Button
17. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=66, PP=132)
18. Change Third Port's "Connected Item" Status From In Use To Available
19. Click Connect Button
20. Click `Connect To VPC A`
21. Click Save Button
22. Go Back To `COOLINGUNITITEM26507` Item Detail
23. Click Refresh Button
24. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=66, PP=132)
25. Change Redundancy From `N+1` To `N`
26. Click Save Button
27. **Verify Values Of Effective Power And Potential Power In Item Detail Are Correct**(EP=66, PP=165)
28. Close tab
29. Open Show/Hide Column
30. Select `Effective Power` and `Potential Power`
31. Click Apply Button
32. **Verify Values Of Effective Power And Potential Power In Items List Are Correct**(EP=66, PP=165)