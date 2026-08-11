TMD-26788 Custom Defined Tooltip for a newly created Custom field in Location details page
## Test Steps
1. Add a new Custom field for Location from Settings-> Field Management -> Custom Fields
2. Go to Settings-> Field Management -> Field Properties
3. Filter 'Tooltip' for 'Location' and 'Custom' for Type from drop-down menus. Verify if the newly created Custom field is displayed.
4. Add a custom tooltip for the custom field and click 'Save' button
5. Go to Assets -> Locations and open an existing location. Verify if the custom defined tooltip are visible for the new Custom field in Location details page.
6. Go to Assets -> Locations -> Add a Location and create a new location. Verify if the custom defined tooltip is visible for the new custom field in Location details page.

## Test Results
1. A new Custom field for Location is added.
2. Field Properties page is loaded.
3. The created Custom field is displayed in Field Properties page.
4. The custom tooltip is saved correctly in Field Properties page.
5. The defined custom tooltip for the new custom field is visible in Location details page when hovering over the field itself.
6. The defined custom tooltip for the new custom field is visible in Location details page when hovering over the field itself.