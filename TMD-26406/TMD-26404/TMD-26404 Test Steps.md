**Goal**
TMD-26404 Check Manifold subclass in Color Code options for Subclass field

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
1. Go To Floor Maps Page
2. Click Color Button
3. **Verify Manifold Subclass Exists In Color Code List Of Floor Maps Page**
   1. Input Item Field : `Subclass`
   2. Open Field Picks dropdown
   3. Click Unselect All
   4. Filter Manifold
   5. Verify Manifold Is Visible In Dropdown
   6. Click Apply Button
   7. Verify Manifold Item Is Visible In Color Code List Grid