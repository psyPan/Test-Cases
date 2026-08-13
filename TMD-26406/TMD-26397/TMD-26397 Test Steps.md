**Goal**
TMD-26397 Check the manifold subclass in various screens
---
## Test Data
### Model
- `Class` : `HVAC`
- `Subclass` : `Manifold`
- `Make` : `3Com`
- `Model Name` : `ManifoldModel26406`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

### Items
#### Item 1 (Create during case setup)
- `Make` : `3Com`
- `Model` : `ManifoldModel26406`
- `Name` : `MANIFOLDITEM26406`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

#### Item 2 (Create using UI In Project-Items Subtab)
- `Make` : `3Com`
- `Model` : `ManifoldModel26406`
- `Name` : `MANIFOLDITEM26397`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

### Project
- `Project Number` : `PRJ26397`
- `Project Name` : `PROJECT26397`
- `Location` : `SITE A`


## Test Steps
1. Go To Items List Page
2. **Verify Manifold Items Are Visible In Project-Items Subtab After Adding With Different Methods**
   1. Open `MANIFOLDITEM26406` With Edit Mode
   2. Click Asset and Maintenance Subtab
   3. Click Project Number Field
   4. Select `PRJ26397`
   5. Save Item
   6. Go To Project Page
   7. Open `PROJECT26397` With Edit Mode
   8. Click Items Subtab
   9. Click Add An Item
   10. Create Item `MANIFOLDITEM26397`
   11. Save Item
   12. Both Items Should Be Visible In Project-items Subtab
3. **Verify Manifold Subclass Is Visible In Subclass Dropdown Of Item Selection Grid When Creating Or Modifiying A Circuit**
   1. Go To Circuit Management Page
   2. Open `NEWPDU-7J-485737:Inlet 1` With Edit Mode
   3. Click First Node
   4. Open Subclass Dropdown In Item Selection Grid
   5. Verify Manifold Is Visible Under HVAC Class
   6. Close Circuit Without Saving
   7. Click Add a Circuit Button
   8. Open Subclass Dropdown In Item Selection Grid
   9. Verify Manifold Is Visible Under HVAC Class
4. **Verify Manifold Subclass Is Visible In Ticket-Items Subtab**
   1. Go To Tickets Page
   2. Click Add a Ticket Button
   3. Input Ticket Number `Ticket26397`
   4. Save Ticket
   5. Click Ticket-Items Subtab
   6. Click Assign an Item Button
   7. Input HVAC In Class Dropdown
   8. Input Manifold In Subclass Dropdown
   9. Select Item `MANIFOLDITEM26406`
   10. Click Select Items Button
   11. Verify Manifold Item Is Visible On Grid
5. **Verify Manifold Subclass Is Visible In Subclass Dropdown Of Item Selection Grid In Data Network Diagram Page**
   1. Go To Data Network Diagram Page
   2. Click Subclass Dropdown
   3. Verify Manifold Subclass Under HVAC Class Is Visible
6. **Verify Custom Field Features Of HVAC Manifold Subclass In Field Management Page**
   1. Setup In Field Management Page
      1. Go to Field Management Page
      2. Click Custom Fields Subtab
      3. Create Custom Field For HVAC/Manifold Subclass Item
         1. Input Custom Field Label : `fieldManifoldItem26397`
         2. Select applies to : `Item`
         3. Select Class (Subclass) : `HVAC/Manifold`
         4. Select Type : `Text`
         5. Click Add Button
      4. Create Custom Field For All Classes Item
         1. Input Custom Field Label : `fieldAllItem26397`
         2. Select applies to : `Item`
         3. Select Class (Subclass) : `Check All`
         4. Select Type : `Text`
         5. Click Add Button
      5. Create Custom Field For HVAC/Manifold Subclass Model
         1. Input Custom Field Label : `fieldManifoldModel26397`
         2. Select applies to : `Item Model`
         3. Select Class (Subclass) : `HVAC/Manifold`
         4. Select Type : `Text`
         5. Click Add Button
      6. Click Design Subtabs
      7. Click Add a Subtab
         1. Subtab title : `subtabItem26397`
         2. Select `Item`
         3. Click Add Button
      8. Click Add a Subtab
         1. Subtab title : `subtabModel26397`
         2. Select `Item Model`
         3. Click Add Button
      9.  Select `subtabItem26397`
      10. Click Add a Panel Button
      11. Drag Custom Fields `fieldManifoldItem26397` and `fieldAllItem26397` into New Panel
      12. Select `subtabModel26397`
      13. Click Add a Panel Button
      14. Drag Custom Field `fieldManifoldModel26397` into New Panel
   2. Verify Filter Function of Identify Button For Custom Fields Inside Panel Grid
      1. Click Identify Button
      2. Select `HVAC/Manifold` option in dropdown
      3. Verify input fields beside `fieldAll26397` and `fieldHVAC26397` turn green
      4. Select `Network/Blade` option in dropdown
      5. Verify just input field of `fieldAll26397` turns green
7. **Verify New Created Custom Fields Are Visible In Item Detail Of Manifold Subclass**
   1. Go To Items List Page
   2. Open Item `MANIFOLDITEM26406` with view mode
   3. Verify `subtabItem26397` subtab is visible
   4. Click `subtabItem26397` subtab
   5. Verify Custom Fields `fieldAllItem26397` and `fieldManifoldItem26397` are visible.
8. **Verify New Created Custom Subtab And Custom Field Are Visible In Model Detail Of Manifold Subclass**
   1. Go To Models Library Page
   2. Open Item `ManifoldModel26406` with view mode
   3. Verify `subtabModel26397` subtab is visible
   4. Click `subtabModel26397` subtab
   5. Verify Custom Field `fieldManifoldModel26397`is visible.