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
#### Item 1
- `Make` : `3Com`
- `Model` : `ManifoldModel26406`
- `Name` : `MANIFOLDITEM26397-1`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

#### Item 2
- `Make` : `3Com`
- `Model` : `ManifoldModel26406`
- `Name` : `MANIFOLDITEM26397-2`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

### Project
- `Project Number` : `PRJ26397`
- `Project Name` : `PROJECT26397`
- `Location` : `SITE A`

### Circuits
#### Circuit 1
- 
---
## Test Steps
1. **Verify Manifold Items Are Visible In Project-Items Subtab After Adding With Different Methods**
   1. Open `MANIFOLDITEM26397-1` With Edit Mode
   2. Click Asset and Maintenance Subtab
   3. Click Project Number Field
   4. Select `PRJ26397`
   5. Save Item
   6. Go To Project Page
   7. Open `PROJECT26397` With Edit Mode
   8. Click Items Subtab
   9. Click Add An Item
   10. Create Item `MANIFOLDITEM26397-2`
   11. Save Item
   12. Both Items Should Be Visible In Project-items Subtab
2.  