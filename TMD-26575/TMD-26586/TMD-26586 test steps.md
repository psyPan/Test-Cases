**Goal**
TMD-26585 Verify Heat Rejection import template contains required capacity and flow columns

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

### Imported Models
#### Model A (All fields valid, Fluid Flow Rate blank)
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HEATREJECTIONITEM26586-1`
- `Make` : `3Com`
- `Location` : `Site A`
- `Nominal Capacity (Tons)` : `100`
- `Airflow Rate (cfm)` : `100`
- `Fluid Flow Rate` : `Empty`

#### Model B (Fluid Flow Rate populated with a valid value (> 0, up to 2 decimals))
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-2`
- `Make` : `3Com`
- `Location` : `Site A`
- `Fluid Flow Rate` : `123.45`

#### Model C (Fluid Flow Rate = 0)
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-3`
- `Make` : `3Com`
- `Location` : `Site A`
- `Fluid Flow Rate` : `0`

#### Model D (Fluid Flow Rate is negative)
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-4`
- `Make` : `3Com`
- `Location` : `Site A`
- `Fluid Flow Rate` : `-9`

#### Model E (Fluid Flow Rate has more than 2 decimals)
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-5`
- `Make` : `3Com`
- `Location` : `Site A`
- `Fluid Flow Rate` : `12.345`

#### Model F (Invalid Compensation Factor)
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-5`
- `Make` : `3Com`
- `Location` : `Site A`
- `Compensation Factor` : `0`

#### Model G (Invalid Nominal Capacity (Tons))
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-5`
- `Make` : `3Com`
- `Location` : `Site A`
- `Nominal Capacity (Tons)` : `0`

#### Model H (Invalid Nominal Capacity (kW))
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-5`
- `Make` : `3Com`
- `Location` : `Site A`
- `Nominal Capacity (kW)` : `0`

#### Model I (Invalid Airflow Rate (cfm) (≤ 0 or invalid format))
- `Operation` : `ADD`
- `Object` : `HEAT REJECTION-RACKABLE`
- `Name` : `HeatRejectionModel26586-5`
- `Make` : `3Com`
- `Location` : `Site A`
- `Airflow Rate (cfm)` : `0`
---
## Test Steps
1. Go To File Import Library
2. Import File
3. Verify Model A And B Are Imported Successfully And Models Are Created/Updated Correctly
4. Verify Model C And D Failed With Validation Error Indicating Values Must Be Greater Than 0
5. Verify Model E Enforced Numeric(10,2) Behavior
6. Verify Model F-I Failed With Same Validation Behaviors And Error Messages