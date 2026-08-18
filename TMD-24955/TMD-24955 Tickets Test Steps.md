**Goal**
TMD-24956 Check the field's label in the tooltip or any existing tooltip is separated by a period from the Custom Tooltip
TMD-24957 Check that the displayed tooltip text matches exactly what the user entered.
TMD-24959 Verify when the details page in view or edit modes of Items, Circuits, projects, tickets, locations, item Models, parts and Part Model is hovered
TMD-26786 Custom Defined Tooltip for all Standard fields in Location details page
TMD-26787 Custom Defined Tooltip for all existing Custom fields in Location details page
TMD-26788 Custom Defined Tooltip for a newly created Custom field in Location details page

## Test Data
### Ticket
- `Ticket Number` : `Ticket24955`

### Tooltips
#### Ticket
- Standard Fields
   - `External System` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Ticket Number` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Summary` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Ticket Type` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Ticket Purpose` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Location` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `dcTrack Status` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Status Date` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Due Date` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Priority` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Severity` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Project Number` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `Assigned To` : `\/ 哈囉 très bien teşekkürler tschüss 24955`

- Existing Custom Fields
   - `Ticket_CF_checkbox` : `\/ 哈囉 très bien teşekkürler tschüss 24955`

- Newly Created Custom Fields
   - `TextCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `TextAreaCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `NumericCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `DateCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `CheckboxCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `SingleSelectCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `MultiSelectCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `TagsCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`
   - `ContactsCustomField24955` : `\/ 哈囉 très bien teşekkürler tschüss 24955`

## Test Steps
1. Add Newly Created Custom Fields Inside Subtab
   1. Go To Field Management Page/Design Subtabs
   2. Filter `Ticket` in Applies To Column
   3. Select `Custom Fields`
   4. Create New Panel And Drag Newly Created Custom Fields Into That Panel
2. **Verify Custom Tooltips Can Be Created In Field Properties Subtab Of Field Management Page**
   1. Go To Field Management Page/Field Properties
   2. Input `Tooltip`, For `Ticket` In Dropdown
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
3. Go To Tickets Page
4. **Verify Fields In Ticket Detail View Mode Page Displays Custom Tooltip**
   1. Open Ticket `Ticket24955` with View Mode
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Existing Custom Field
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   5. Close Ticket
5. **Verify Fields In Ticket Detail Edit Mode Page Displays Custom Tooltip**
   1. Open Ticket `Ticket24955` with Edit Mode
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Existing Custom Field
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   5. Close Ticket
6. **Verify Fields In Create A Ticket Page Displays Custom Tooltip**
   1. Click Add a Ticket
   2. Verify Custom Tooltip Of Standard Fields
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   3. Verify Custom Tooltip Of Existing Custom Field
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period
   4. Verify Custom Tooltip Of Newly Created Custom Fields Of Different Types
      1. Verify Fields Have Custom Tooltip
      2. Verify Field Label Is Separated From Custom Tooltip By A Period