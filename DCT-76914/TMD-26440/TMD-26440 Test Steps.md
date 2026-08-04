**Goal**
TMD-26440 Verify a new column called "Derate Amps" is added to the import sheet for adding and editing breakers
---
## Test Data
### Create FPDU Item
- `Make` : `APC`
- `Model` : `0G-PD80G6FK1`
- `Name` : `FPDUITEM26440`
- `Status` : `Planned`
- `Location` : `SITE A`

#### Create Local Power Panel In `FPDUITEM26440`
- `Object` : `POWER PANEL-LOCAL`
- `Floor PDU` : `FPDUITEM26440`
- `Name` : `LOCALPANEL`
- `Location` : `SITE A`
- `Phases` : `Single Phase (3-Wire)`
- `Phase Volts` : `120`
- `Wire Colors` : `Black/Red`
- `Rating (A)` : `100`
- `No of Poles` : `40`
- `Panel Layout` : `Two Column`
- `Pole Numbering` : `Odd/Even`

#### Create Remote Power Panel In `FPDUITEM26440`

### Create Plant Item
- `Make` : `Generic`
- `Model` : `Plant`
- `Name` : `PLANTITEM26440`
- `Status` : `Planned`
- `Location` : `SITE A`
- `Battery Recharge Factor (%)` : `80`
- `Engineered Capacity (A)` : `2960`
- `Output Volts (Vdc)` : `24`

### Create DC Bay Item
- `Make` : `Emerson`
- `Model` : `801DB`
- `Name` : `DCBAYITEM26440`
- `Status` : `Planned`
- `Location` : `SITE A`

---
## Test Steps