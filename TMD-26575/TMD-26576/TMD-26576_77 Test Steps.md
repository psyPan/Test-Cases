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
6. Input `Compensation Factor`: `0`
7. **Verify Validation Error Is Visible**
8. **Verify Save Button Is Disabled**
9. Input `Compensation Factor`: `201`
10. **Verify Validation Error Is Visible**
11. **Verify Save Button Is Disabled**
12. Input `Compensation Factor`: `120`
13. **Verify Warning Icon Is Visible Beside Compensation Factor Label**
14. Click Save Button
15. **Verify Model Can be Saved With Compensation Factor Value From 101 To 200**
16. **Verify Warning Icon Is Not Visible For Compensation Factor Value From 1 To 100**
    1.  Input `Compensation Factor`: `50`
    2.  **Verify Warning Icon Is Not Visible Beside Compensation Factor Label**
    3.  Click Save Button