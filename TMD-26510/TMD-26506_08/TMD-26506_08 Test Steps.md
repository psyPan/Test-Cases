**Goal**
TMD-26506 Verify Potential Power and Effective Power fields for Cooling Unit
TMD-26508 Verify the auto power budget fields
---
## Test Steps
1. Go To Models Library Page
2. Open Show/Hide Column
3. Search `Original Power`
4. **Verify Original Power Option Under HVAC Class Is Not Visible** 
(//*[contains(normalize-space(), 'Show/Hide Columns')]//*[(@class='ng-hide') and (contains(normalize-space(), 'HVAC'))])
5. Repeat 3. and 4. for `Budget Status` and `Auto Power Budget`
6. Open Model `AP7003`
7. Click `Power Supply Ports` Subtab
8. **Verify Original Power, Budget Status and Auto Power Budget Field Is Not Visible**
(TMD-17784     
Items List::Open Item With Edit Mode    ${itemName}
Item Detail::Wait Until Subtab Field Is Not Visible    ${dataCircuitCustomField17791.name}
Items List::Close Tab    ${itemName}
Items List::Click Clear Button)
9. Close Tab
10. Go To Items List Page
11. Open Show/Hide Column
12. Search `Original Power`
13. **Verify Original Power Option Under HVAC Class Is Not Visible**
14.
14. Repeat 12. and 13. for `Budget Status` and `Auto Power Budget`
15. Open Item `ARAC1`
16. Click `Power Supply Ports` Subtab
17. **Verify Original Power, Budget Status and Auto Power Budget Field Is Not Visible**

