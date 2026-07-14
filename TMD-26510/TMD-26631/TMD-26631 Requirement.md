TMD-26492 Import Validation Rules
## Test Steps
1. Verify that in the Model List and Assets List, the field is not shown by default, but can be added via the Show/Hide Columns UI.

2. In Settings → Field Management → Standard Fields, the field should be visible for Items and Models.

3. In Settings → Field Management → Field Properties, verify that for Items and Models the field has these properties:
Required - Unchecked/Editable
Hidden - Unchecked/Editable
Default - Allowed/Configurable
Must be Unique - Unchecked/ Read Only

## Test Results
The field is present in the Field Management menus and has correct properties.