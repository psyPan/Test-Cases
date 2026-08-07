**Goal**
TMD-26398 Check parts assignment to Manifolds
TMD-26399 Check Manifold subclass in Floor Maps
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
1. Go To Parts Page
2. **Verify Manifold Subclass Is Visible And Selectable In Dropdown Menu Under Assignment Subtab In Part Management**
   1. Click Add Part(s)
   2. Select `Avaya RPS15 PSU / PSE2-115/230-IS-073` In Model / Part Number Field
   3. Open Subclass Dropdown In Assignments Subtab
   4. Manifold Subclass Should Be Visible And Selectable As A Subclass Of HVAC
3. **Verify Manifold Subclass Is Visible Under Subclass Column In Search Results Grid Of Floor Maps Page**
   1. Go To Floor Maps Page
   2. Open Show/Hide Columns
   3. Select `Subclass` And Click Apply
   4. Filter In Search Bar: title=Hardware, field=Subclass, value=Manifold
   5. Manifold Subclass Items Should Be Visible And Selectable In Search Results Grid