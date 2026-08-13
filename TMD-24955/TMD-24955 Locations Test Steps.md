**Goal**
TMD-24956 Check the field's label in the tooltip or any existing tooltip is separated by a period from the Custom Tooltip
TMD-24957 Check that the displayed tooltip text matches exactly what the user entered.
TMD-24959 Verify when the details page in view or edit modes of Items, Circuits, projects, tickets, locations, item Models, parts and Part Model is hovered
TMD-26786 Custom Defined Tooltip for all Standard fields in Location details page
TMD-26787 Custom Defined Tooltip for all existing Custom fields in Location details page
TMD-26788 Custom Defined Tooltip for a newly created Custom field in Location details page

## Test Data
### Tooltips
#### Location
- Standard Fields
   - `Node Code` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Level in Hierarchy` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Parent` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Description` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Type` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Owner` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Can Contain Assets` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Power Capacity (kW)` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Power IQ Host Association` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `VM Manager` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `AC Virtual Power Chain` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `DC Virtual Power Chain` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `System Default Location` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - Address Subtab -> `Country` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - Dimensions Subtab -> `Area` : `\/ 哈囉 très bien teşekkürler tschüss 24955`

- Existing Custom Fields
   - `Company Name` : `\/ 哈囉 très bien teşekkürler tschüss 24955`

- Newly Created Custom Fields
   - `TextCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955` chinese, france/german, turkish
   - `TextAreaCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `NumericCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `DateCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `CheckboxCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `SingleSelectCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `MultiSelectCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `TagsCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `ContactsCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`

## Test Steps
1. **Verify Custom Tooltips Can Be Created In Field Properties Subtab Of Field Management Page**
   1. Go To Field Management Page/Field Properties
   2. Input `Tooltip`, For `Location` In Dropdown
   3. **Verify Custom Tooltips For Standard Fields Can Be Created**
      1. Filter `Standard` In Type Column
      2. Verify Only Standard Fields Are Displayed
      3. Input Tooltip `\/ 哈囉 très bien teşekkürler tschüss 24955` For Standard Fields In Test Data
      4. Click Save Button
   4. **Verify Custom Tooltips For Custom Fields Can Be Created**
      1. Filter `Custom` In Type Column
      2. Verify Only Custom Fields Are Displayed
      3. Input Tooltip `\/ 哈囉 très bien teşekkürler tschüss 24955` For Existing And Newly Created Custom Fields In Test Data
      4. Click Save Button
2. Add Newly Created Custom Fields Inside Subtab
   1. Go To Field Management Page/Design Subtabs
   2. Filter `Location` in Applies To Column
   3. Select `Custom Fields`
   4. Create New Panel And Drag Newly Created Custom Fields Into That Panel
3. Go To Locations Page
4. **Verify Fields In Location Detail View Mode Page Displays Custom Tooltip**
   1. Open Location `UNITED STATES > SITE A` with View Mode
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Existing Custom Field
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   5. Close Location
5. **Verify Fields In Location Detail Edit Mode Page Displays Custom Tooltip**
   1. Open Location `UNITED STATES > SITE A` with Edit Mode
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Existing Custom Field
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   5. Close Location
6. **Verify Fields In Create A Location Page Displays Custom Tooltip**
   1. Click Add a Location
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Existing Custom Field
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period