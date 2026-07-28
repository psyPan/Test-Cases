**Goal**
TMD-26585 Verify Heat Rejection import template contains required capacity and flow columns

---
## Test Data
### Model
- `Operation` : `ADD`
- `Object` : `MODEL`
- `Make` : `3Com`
- `Model Name` : `HeatRejectionModel26585`
- `Class` : `HVAC`
- `Subclass` : `Heat Rejection`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Rack Units` : `1`
- `Height` : `1`
- `Nominal Capacity (Tons)` : `100`
- `Nominal Capacity (kW)` : `351.69`
- `Compensation Factor (%)` : `100`
- `Airflow Rate (cfm)` : `100`
- `Fluid Flow Rate (gpm)` : `100`

---
## Test Steps
1. Go To File Import Library
2. Click `Item Models Import Template`
3. Open Downloaded File
4. **Verify Columns For Heat Rejection Subclass Are Visible In Models Template**
5. **Verify Fields Of Imported Model Are Same As Import File**
   1. Create Model `HeatRejectionModel26585` By File Import
   2. Go To Models Library Page
   3. Open `HeatRejectionModel26585` With View Mode
6. **Verify Verify Model Fields Are Updated By Edited Import File**
   1. Back To Models Library Page
   2. Click Export Button To Export Details into an Import Template, Group By Model
   3. Change Value In Exported CSV(另一個CSV也行)
      1. Edit `Operation` : `EDIT`
      2. Edit `Compensation Factor` : `90`
      3. Edit `Nominal Capacity (Tons)` : `40`
      4. Edit `Nominal Capacity (kW)` : `140.67`
      5. Edit `Airflow Rate (cfm)` : `130`
      6. Edit `Fluid Flow Rate (gpm)` : `150`
   4. Go To File Import Page
   5. Edit Model `HeatRejectionModel26585` By File Import
   6. Go To Models Library
   7. Open Model `HeatRejectionModel26585` With View Mode
   8. Verify Model Fields Are Updated By Edited Import File