[TMD-26506] Verify Potential Power and Effective Power fields for Cooling Unit
## Test Steps
Create a Cooling Unit item and add power supply ports to it.
Verify that the power supply ports subtab has 2 fields in its header, Potential Power and Effective Power. It should look like in Device items.
Verify also that the fields show in the Items List (may need adding in the grid via the Show/Hide UI).

## Test Results
The fields are present.

[TMD-26508] Verify the auto power budget fields
## Test Steps
In a Cooling Unit with power supply ports, check that the power supply ports subtab does not have the auto power budget fields: Original Power, Budget Status, Auto Power Budget

## Test Results
The fields are not displayed, in Item’s Details and in Items List. Both for Items and Models