TMD-26580 Verify calculation of Sensible Capacity (Tons) based on Compensation Factor (%) and Nominal Capacity (Tons)

## Test step
1. Locate the Sensible Capacity (Tons) field.
2. Enter a valid value in the Compensation Factor (%) field.
3. Enter a valid value in the Nominal Capacity (Tons) field.
4. Сave the model and observe the Sensible Capacity (Tons) field.

## Test Result
After entering values for Compensation Factor (%) and Nominal Capacity (Tons):

-The system automatically calculates the Sensible Capacity (Tons) value.

-The calculated value is populated in the Sensible Capacity (Tons) field.

-The calculation reflects the entered Compensation Factor (%) and Nominal Capacity (Tons) values.

-The model can be saved successfully.


TMD-26581 Verify calculation of Sensible Capacity (kW) based on Compensation Factor (%) and Nominal Capacity (kW)

## Test step
1. Locate the Sensible Capacity (kW) field.
2. Enter a valid value in the Compensation Factor (%) field.
3. Enter a valid value in the Nominal Capacity (kW) field.
4. Save the model and observe the Sensible Capacity (kW) field.

## Test Result
After entering values for Compensation Factor (%) and Nominal Capacity (kW):

-The system automatically calculates the Sensible Capacity (kW) value.

-The calculated value is populated in the Sensible Capacity (kW) field.

-The calculation correctly reflects the entered Compensation Factor (%) and Nominal Capacity (kW) values.

The model can be saved successfully.


TMD-26582 Verify capacity conversion formulas, auto-population, and recalculation across all capacity fields

## Test step
1. Navigate to the Specification subtab.
2. Enter a valid numeric value in one of the Capacity fields (e.g., Nominal Capacity (kW)).
3. Observe the remaining three Capacity fields.
4. Verify that all other Capacity fields are auto-populated.
5. Manually calculate the expected converted values using the formulas above.
   1. kW to tons:   kW number / ( 12,000 X 0.0002930711 )
   2. tons to kW: tons number X 12,000 X 0.0002930711
6. Compare the system-calculated values with the expected results.
7. Edit a different Capacity field (e.g., Nominal Capacity (Tons)).
8. Observe all remaining Capacity fields again.
9.  Repeat the test by editing each of the remaining Capacity fields one at a time.

## Test Result
When a value is entered into any one of the Capacity fields:
-The remaining three Capacity fields are automatically populated.

The populated values:
- Follow the correct conversion formulas: kW ↔ Tons
- Are numerically accurate and within acceptable rounding precision.

When any one of the five fields (including Compensation Factor) is edited:
- The remaining four fields are automatically recalculated.
- All displayed values remain synchronized and consistent.