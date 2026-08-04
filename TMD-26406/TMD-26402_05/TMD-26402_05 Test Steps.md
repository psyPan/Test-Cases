**Goal**
TMD-26402 Test Floor Maps search for Manifold custom field
TMD-26405 Check Manifold subclass in search field in Floor Maps

--- 
## Test Data
### Models
#### Model
- `Class` : `HVAC`
- `Subclass` : `Manifold`
- `Make` : `3Com`
- `Model Name` : `ManifoldModel26406`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

### Item
- `Make` : `3Com`
- `Model` : `ManifoldModel26406`
- `Name` : `MANIFOLDITEM26406`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

---
## Test Steps
1. Go To Items List Page
2. Open `MANIFOLDITEM26406` With Edit Mode
3. Click Custom Fields Subtab
4. Input `HG-text area` `Text26402_05`
5. Save Item
6. Go To Floor Maps Page
7. Click Search Button
8. **Verify Functionality Of Search Bar In Floor Maps Page By Custom Field Value Of Manifold Item**
   1. Input `HG-text area:Text26402_05`
   2. Item With Custom Field Value Should Be Filtered In Search Results Grid
   3. Clear Search Grid
9. **Verify Subclass Manifold Can Be Searched In Floor Maps Page**
   1. Input `Subclass:`
   2. Manifold Should Be Visible And Selectable In Dropdown