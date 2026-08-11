TMD-24957 Check that the displayed tooltip text matches exactly what the user entered.
## Test Steps
1. Open browser.
2. Log in with User role in Test Data.
3. Go to Page1 defined in Test Data.
4. Click Field Properties.
5. Expand the drop-down list that displays "Required" and click the "Custom Tooltip" option.
6. Select any row and record the panel, field, and tooltip text.
7. Go to Page2 defined in Test Data.
8. Double click any item
9. Move the cursor to hover what you recorded.
10. Verify that the displayed tooltip text matches exactly what you recorded. (Keyword -> Tooltip Of More Options Button Should Be)
11. Close browser.

## Test Data
User role: [Administrator]
Page1: [Field Management]
Page2: [Items]

## Test Results
1. Step 10