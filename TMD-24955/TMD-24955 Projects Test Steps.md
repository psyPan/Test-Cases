**Goal**
TMD-24956 Check the field's label in the tooltip or any existing tooltip is separated by a period from the Custom Tooltip
TMD-24957 Check that the displayed tooltip text matches exactly what the user entered.
TMD-24959 Verify when the details page in view or edit modes of Items, Circuits, projects, tickets, locations, item Models, parts and Part Model is hovered
TMD-26786 Custom Defined Tooltip for all Standard fields in Location details page
TMD-26787 Custom Defined Tooltip for all existing Custom fields in Location details page
TMD-26788 Custom Defined Tooltip for a newly created Custom field in Location details page

## Test Data
### Tooltips
#### Project
- Standard Fields
   - `Project Number` : `tooltip24955`
   - `Project Name` : `tooltip24955`
   - `Description` : `tooltip24955`
   - `Location` : `tooltip24955`
   - `Cabinets` : `tooltip24955`
   - `URs` : `tooltip24955`
   - `kW` : `tooltip24955`
   - `Item Cost` : `tooltip24955`
   - `Misc Cost` : `tooltip24955`
   - `Estimated` : `tooltip24955`
   - `Actual` : `tooltip24955`
   - `Status` : `tooltip24955`
   - `Substatus` : `tooltip24955`

- Newly Created Custom Fields
   - `TextCustomField24955` : `tooltip24955`
   - `TextAreaCustomField24955` : `tooltip24955`
   - `NumericCustomField24955` : `tooltip24955`
   - `DateCustomField24955` : `tooltip24955`
   - `CheckboxCustomField24955` : `tooltip24955`
   - `SingleSelectCustomField24955` : `tooltip24955`
   - `MultiSelectCustomField24955` : `tooltip24955`
   - `TagsCustomField24955` : `tooltip24955`
   - `ContactsCustomField24955` : `tooltip24955`

## Test Steps
1. **Verify Custom Tooltips Can Be Created In Field Properties Subtab Of Field Management Page**
   1. Go To Field Management Page/Field Properties
   2. Input `Tooltip`, For `Project` In Dropdown
   3. **Verify Custom Tooltips For Standard Fields Can Be Created**
      1. Filter `Standard` In Type Column
      2. Verify Only Standard Fields Are Displayed
      3. Input Tooltip `tooltip24955` For Standard Fields In Test Data
      4. Click Save Button
   4. **Verify Custom Tooltips For Custom Fields Can Be Created**
      1. Filter `Custom` In Type Column
      2. Verify Only Custom Fields Are Displayed
      3. Input Tooltip `tooltip24955` For Newly Created Custom Fields In Test Data
      4. Click Save Button
2. Add Newly Created Custom Fields Inside Subtab
   1. Go To Field Management Page/Design Subtabs
   2. Filter `Project` in Applies To Column
   3. Select `Custom Fields`
   4. Create New Panel And Drag Newly Created Custom Fields Into That Panel
3. Go To Projects Page
4. **Verify Fields In Project Detail View Mode Page Displays Custom Tooltip**
   1. Open Project `dcTrack 3.0 GA386` with View Mode
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Close Project
5. **Verify Fields In Project Detail Edit Mode Page Displays Custom Tooltip**
   1. Open Project `dcTrack 3.0 GA386` with Edit Mode
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Close Project
6. **Verify Fields In Create A Project Page Displays Custom Tooltip**
   1. Click Add a Project
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period