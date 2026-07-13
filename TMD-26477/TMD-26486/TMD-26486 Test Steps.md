## Test Case
TMD-26486 Fluid Flow Rate field properties in Field Management
---
## Test Steps
1. Go to field management page
2. Click field properties subtab
3. Open Show/Hide columns
4. Select Heat Rejection subclass
5. Filter Fluid Flow Rate in field column
6. Select Required in dropdown
7. **Verify checkbox is unchecked and editable for heat rejection subclass**
8. Select Hidden in dropdown
9. **Verify checkbox is unchecked and editable for heat rejection subclass**
10. Select Default in dropdown
11. **Verify field is allowed and configurable for heat rejection subclass**(tag-> Single Process Only??)
    - Input Value in the field
    - Click Save button
    - Verify Value Is Set In Field
    - Change Value Back To Empty
12. Select Must Be Unique in dropdown
13. **Verify checkbox is unchecked and readonly for heat rejection subclass**