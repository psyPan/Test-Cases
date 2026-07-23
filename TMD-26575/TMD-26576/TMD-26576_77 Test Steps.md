**Goal**
TMD-26576 Verify that Heat Rejection subclass models have a Specification subtab with all required fields
TMD-26577 Verify validation, boundaries, and warning behavior for Compensation Factor (%) field

---
## Test Data
### Model
- `Class` : `HVAC`
- `Subclass` : `Heat Rejection`
- `Make` : `3Com`
- `Model Name` : `HeatRejectionModel26575`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

---
## Test Steps
1. Go To Models Library
2. Open Model `HeatRejectionModel26575` With Edit Mode
3. Click Specification Subtab
4. **Verify Certain Fields Under Specification Subtab Are Visible, Correctly Labeled And Not Duplicated In Model Detail**(For Not Duplicated -> Use "Get Element Count")
5. **Verify Compensation Factor Field Is Marked As Required**
6. Input `Compensation Factor` `0`
7. 