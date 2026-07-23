TMD-26582 Verify capacity conversion formulas, auto-population, and recalculation across all capacity fields

## Test step
1. Navigate to the Specification subtab.
2. Enter a valid numeric value in one of the Capacity fields (e.g., Nominal Capacity (kW)).
3. Observe the remaining three Capacity fields.
4. Verify that all other Capacity fields are auto-populated.
5. Manually calculate the expected converted values using the formulas above.
6. Compare the system-calculated values with the expected results.
7. Edit a different Capacity field (e.g., Nominal Capacity (Tons)).
8. Observe all remaining Capacity fields again.
9. Repeat the test by editing each of the remaining Capacity fields one at a time.

## Test Result
When a value is entered into any one of the Capacity fields:
-The remaining three Capacity fields are automatically populated.

The populated values:
- Follow the correct conversion formulas: kW ↔ Tons
- Are numerically accurate and within acceptable rounding precision.

When any one of the five fields (including Compensation Factor) is edited:
- The remaining four fields are automatically recalculated.
- All displayed values remain synchronized and consistent.