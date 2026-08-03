**Goal**
TMD-26398 Check parts assignment to Manifolds
TMD-26399 Check Manifold subclass in Floor Maps
--- 
## Test Data
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
1. **Verify Manifold Subclass Is Visible As A Subclass Of HVAC In Dropdown Menu In Assignment Subtab In Part Management**
   1. Click Add Part(s)
   2. Select `Avaya RPS15 PSU / PSE2-115/230-IS-073` In Model / Part Number Field
   3. Open Subclass Dropdown In Assignments Subtab
   4. Manifold Subclass Should Be Visible As A Subclass Of HVAC
2. **Verify Manifold Subclass Is Visible Under Subclass Column In Items List Of Floor Maps Page**
   1. Open Show/Hide Columns
   2. Select `Subclass` And Click Apply
   3. Manifold Subclass Should Be Visible And Selectable