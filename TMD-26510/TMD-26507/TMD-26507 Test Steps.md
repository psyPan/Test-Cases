**Goal**
TMD-26507 Verify the values of Effective Power and Potential Power fields for Cooling Unit
---
## Test Data
### Item
#### Create Item
- `Make` : `APC`
- `Model` : `APC1000`
- `Name` : `COOLINGUNITITEM26507`
- `Status` : `Planned`
- `Location` : `Site A`

## Test Steps
1. Create Power Supply Ports By File Import 
2. Go To Item List Page
3. Click "Show/Hide Column"
4. Select "Effective Power(W)" And "Potential Power(W)"
5. **Verify Values Of Effective Power And Potential Power In Items List Are Correct** (EP=0, PP=132)
6. Open Item `COOLINGUNITITEM26507` With Edit Mode
7. Click "Power Supply Ports" Subtab
8. **Verify Values Of Effective Power And Potential Power In Items Detail Are Correct**(EP=0, PP=132)
9. Change Second Port's "Connected Item" Status From Available To In Use
10. Click Save Button
11. **Verify Values Of Effective Power And Potential Power In Items Detail Are Correct**(EP=33, PP=132)
12. Close tab
13. **Verify Values Of Effective Power And Potential Power In Items List Are Correct**(EP=33, PP=132)
14. Open Item `COOLINGUNITITEM26507` With Edit Mode
15. Click "Power Supply Ports" Subtab
16. Change Third Port's "Connected Item" Status From Available To In Use
17. Click Save Button
18. **Verify Values Of Effective Power And Potential Power In Items Detail Are Correct**(EP=66, PP=132)
19. Close tab
20. **Verify Values Of Effective Power And Potential Power In Items List Are Correct**(EP=66, PP=132)
21. Open Item `COOLINGUNITITEM26507` With Edit Mode
22. Click "Power Supply Ports" Subtab
23. Change Third Port's "Connected Item" To Connect VPC A Item
17. Click Save Button
18. **Verify Values Of Effective Power And Potential Power In Items Detail Are Correct**(EP=66, PP=132)
19. Close tab
20. **Verify Values Of Effective Power And Potential Power In Items List Are Correct**(EP=66, PP=132)
21. Open Item `COOLINGUNITITEM26507` With Edit Mode
22. Click "Power Supply Ports" Subtab
23. Change "Redundancy" Value From "N+1" To "N"
24. Click Save Button
25. **Verify Values Of Effective Power And Potential Power In Items Detail Are Correct**(EP=66, PP=165)
26. Close tab
27. **Verify Values Of Effective Power And Potential Power In Items List Are Correct**(EP=66, PP=165)