**Goal**
TMD-26580 Verify calculation of Sensible Capacity (Tons) based on Compensation Factor (%) and Nominal Capacity (Tons)
TMD-26581 Verify calculation of Sensible Capacity (kW) based on Compensation Factor (%) and Nominal Capacity (kW)
TMD-26582 Verify capacity conversion formulas, auto-population, and recalculation across all capacity fields

## Test Data
### Model
- `Class` : `HVAC`
- `Subclass` : `Heat Rejection`
- `Make` : `3Com`
- `Model Name` : `HeatRejectionModel26575`
- `Mounting` : `Rackable`
- `Form Factor` : `Fixed`
- `Height` : `1`

## Test Steps
1. Go To Models Library
2. Open Model `HeatRejectionModel26575` With Edit Mode
3. **Verify All Capacity Fields And Compensation Factor Are Synchronized And Consistent When Nominal Capacity (Tons) Value Is Edited**
   1. Input `Compensation Factor (%)`: `50` And `Nominal Capacity (Tons)`: `100`
   2. **Compensation Factor Should Be**    (50)
   3. **Nominal Capacity (Tons) Should Be**    (100)
   4. **Nominal Capacity (kW) Should Be**    (351.69)
   5. **Sensible Capacity (Tons) Should Be**    (50)
   6. **Sensible Capacity (kW) Should Be**    (175.85)
4. **Verify Sensible Capacity (Tons) Is Product Of Compensation Factor (%) And Nominal Capacity (Tons)**
   - **Sensible Capacity (Tons) Should Be**    (50)    # TMD-26580 done here
5. Input `Nominal Capacity (kW)`: `100`
6. **Verify All Capacity Fields And Compensation Factor Are Synchronized And Consistent When Nominal Capacity (kW) Value Is Edited**
   1. **Compensation Factor Should Be**    (50)
   2. **Nominal Capacity (Tons) Should Be**    (28.43)
   3. **Nominal Capacity (kW) Should Be**    (100)
   4. **Sensible Capacity (Tons) Should Be**    (14.22)
   5. **Sensible Capacity (kW) Should Be**    (50)
7.  **Verify Sensible Capacity (kW) Is Product Of Compensation Factor (%) And Nominal Capacity (kW)**
   - **Sensible Capacity (kW) Should Be**    (50)    # TMD-26581 done here
8.  Input `Sensible Capacity (kW)`: `200`
9.  **Verify Verify All Capacity Fields And Compensation Factor Are Synchronized And Consistent When Sensible Capacity (kW) Value Is Edited**
   1. **Compensation Factor Should Be**    (200)
   2. **Nominal Capacity (Tons) Should Be**    (28.43)
   3. **Nominal Capacity (kW) Should Be**    (100)
   4. **Sensible Capacity (Tons) Should Be**    (56.86)
   5. **Sensible Capacity (kW) Should Be**    (200)
10. Input `Sensible Capacity (Tons)`: `28.43`
11. **Verify Verify All Capacity Fields And Compensation Factor Are Synchronized And Consistent When Sensible Capacity (Tons) Value Is Edited**
   1. **Compensation Factor Should Be**    (100)
   2. **Nominal Capacity (Tons) Should Be**    (28.43)
   3. **Nominal Capacity (kW) Should Be**    (99.98)
   4. **Sensible Capacity (Tons) Should Be**    (28.43)
   5. **Sensible Capacity (kW) Should Be**    (99.98)
12. Input `Compensation Factor`: `25`
13. **Verify Verify All Capacity Fields And Compensation Factor Are Synchronized And Consistent When Compensation Factor Value Is Edited**
   1. **Compensation Factor Should Be**    (25)
   2. **Nominal Capacity (Tons) Should Be**    (28.43)
   3. **Nominal Capacity (kW) Should Be**    (99.98)
   4. **Sensible Capacity (Tons) Should Be**    (7.11)
   5. **Sensible Capacity (kW) Should Be**    (25)