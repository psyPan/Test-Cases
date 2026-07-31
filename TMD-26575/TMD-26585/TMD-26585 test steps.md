**Goal**
TMD-26585 Verify Heat Rejection import template contains required capacity and flow columns

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

## Test Steps
1. Go To File Import Page
2. Click `Item Models Import Template`
3. Open Downloaded File
4. **Verify Column Headers For Heat Rejection Subclass Are Visible In Models Template**
5. **Verify Fields Values Of Imported Model Are Same As Import File**
   1. Create Model `HeatRejectionModel26585` By File Import
   2. Go To Models Library Page
   3. Open `HeatRejectionModel26585` With View Mode
   4. Verify Model Fields
6. **Verify Fields Values Of Exported File Are Same As Model's**
   1. Back To Models Library Page
   2. Click Export Button To Export Details into an Import Template, Group By Model
   3. Verify Column Headers In Exported File
   4. Verify Model Fields Values In Exported File
7. **Verify Model Fields Value Can Be Edited By File Import**
   1. Fill Value In CSV
      1. `Operation` : `EDIT`
      2. `Compensation Factor` : `90`
      3. `Nominal Capacity (Tons)` : `40`
      4. `Nominal Capacity (kW)` : `140.67`
      5. `Airflow Rate (cfm)` : `130`
      6. `Fluid Flow Rate (gpm)` : `150`
   2. Go To File Import Page
   3. Edit Model `HeatRejectionModel26585` By File Import
   4. Go To Models Library
   5. Open Model `HeatRejectionModel26585` With View Mode
   6.  Verify Model Fields Are Updated