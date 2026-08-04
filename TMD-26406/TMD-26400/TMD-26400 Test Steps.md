**Goal**
TMD-26400 Test subclass change in existing Manifold model
--- 
## Test Data
### Models
#### Model 1 (Existing Model)
- `Class` : `HVAC`
- `Subclass` : `Manifold`
- `Make` : `3Com`
- `Model Name` : `ManifoldModel26406`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

#### Model 2 (New Model)
- `Class` : `HVAC`
- `Subclass` : `Cooling Unit`
- `Make` : `3Com`
- `Model Name` : `ManifoldModel26400`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

#### Item 1
- `Make` : `3Com`
- `Model` : `ManifoldModel26406`
- `Name` : `MANIFOLDITEM26406`
- `Status` : `Planned`
- `Location` : `Site A`
- `Cabinet` : `1A`
- `U Position` : `Above`

## Test Steps
1. **Verify Error Message Is Visible When Changing In Use Model's Subclass**
   1. Open Model `ManifoldModel26406` With Edit Mode
   2. Change Subclass To Cooling Unit
   3. Save Model
   4. Error Message Should Be Visible
2. **Verify Subclass Can Be Changed On Newly Created Model**
   1. Open Model `ManifoldModel26400` With Edit Mode
   2. Change Subclass To Manifold
   3. Save Model
   4. Model Should Be Saved