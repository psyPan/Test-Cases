**Goal**
TMD-26578 Verify auto-calculation of Nominal Capacity (Tons) when Nominal Capacity (kW) is entered first
TMD-26579 Verify auto-calculation of Nominal Capacity (kW) when Nominal Capacity (Tons) is entered first

---
## Test Data
### Model
- `Class` : `HVAC`
- `Subclass` : `Heat Rejection`
- `Make` : `3Com`
- `Model Name` : `HeatRejectionModel26578_79`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

---
## Test Steps
1. Go To Models Library
2. Click Add A Model Button
3. Input Model's Information
   - `Class` : `HVAC`
   - `Subclass` : `Heat Rejection`
   - `Make` : `3Com`
   - `Model Name` : `HeatRejectionModel26578_79`
   - `Mounting` : `Rackable`
   - `Form Factor` : `Fixed`
   - `Height` : `1`
4. **Verify Nominal Capacity (Tons) Value Can Be Empty**
   1. **Verify Nominal Capacity (Tons) Is Not Required Field**
   2. Input Empty Value To Nominal Capacity (Tons)
   3. Move Mouse Over Nominal Capacity (Tons) Input Field
   4. Validation Error Is Not Visible
5. Click Save Button
6. **Verify Nominal Capacity (Tons) Is Correctly Calculated From Nominal Capacity (kW)**
   1. Input `Nominal Capacity (kW)` `100`
   2. Click Save Button
   3. Nominal Capacity (Tons) Value Should Be `28.43`
7. **Verify Nominal Capacity (kW) Value Can Be Empty**
   1. **Verify Nominal Capacity (kW) Is Not Required Field**
   2. Input Empty Value To Nominal Capacity (kW)
   3. Move Mouse Over Nominal Capacity (kW) Input Field
   4. Validation Error Is Not Visible
8. Click Save Button
9.  **Verify Nominal Capacity (kW) Is Correctly Calculated From Nominal Capacity (Tons)**
   1. Input `Nominal Capacity (Tons)` `100`
   2. Click Save Button
   3. Nominal Capacity (Tons) Value Should Be `351.69`