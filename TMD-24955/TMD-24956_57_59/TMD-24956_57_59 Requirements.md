TMD-24956 Check the field's label in the tooltip or any existing tooltip is separated by a period from the Custom Tooltip
## Test Steps
1. Open browser.
2. Log in with User role in Test Data.
3. Go to Pages define in Test Data.
4. Double click any row.
5. Move the cursor to hover any of the field's label.
6. Verify that the field's label in the tooltip or any existing tooltip is separated by a period from the Custom Tooltip.
7. Close browser.

## Test Data
User role: 
[Administrator]
Pages: 
[Items]

## Test Results
1. Step 5
---
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
---
TMD-24959 Verify when the details page in view or edit modes of Items, Circuits, projects, tickets, locations, item Models, parts and Part Model is hovered
## Test Steps
1. Open browser.
2. Log in with User role in Test Data.
3. Go to Pages define in Test Data.
4. Double click any row.
5. Move the cursor to hover any of the field's label.
6. Verify there is a Field Name the same as the text in label in the appearing tooltip.
7. Verify there is any Standard tooltip added for the field in the appearing tooltip. 
8. Verify there is a Custom Tooltip added in field management for this field in the appearing tooltip.
9. Click the "Edit" button.
10. Move the cursor to hover any of the field's label.
11. Verify there is a Field Name the same as the text in label in the appearing tooltip.
12. Verify there is any Standard tooltip added for the field in the appearing tooltip.
13. Verify there is a Custom Tooltip added in field management for this field in the appearing tooltip.
14. Close browser.

## Test Results
1. Step 6, Step 7, Step 8, Step 11, Step 12, Step 13