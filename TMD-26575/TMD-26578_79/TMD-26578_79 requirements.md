TMD-26578 Verify auto-calculation of Nominal Capacity (Tons) when Nominal Capacity (kW) is entered first

## Test step
1. Locate the Nominal Capacity (Tons) field on the Specification subtab.
2. Verify that the Nominal Capacity (Tons) field is optional.
3. Leave the Nominal Capacity (Tons) field empty.
4. Enter a valid numeric value in the Nominal Capacity (kW) field.
5. Move focus out of the Nominal Capacity (kW) field or save the model.
6. Observe the Nominal Capacity (Tons) field.
   1. kW to tons:   kW number / ( 12,000 X 0.0002930711 )
   2. tons to kW: tons number X 12,000 X 0.0002930711

## Test Result
The Nominal Capacity (Tons) field is displayed and is not marked as required.

When Nominal Capacity (kW) is entered first:
- The system automatically calculates the corresponding value for Nominal Capacity (Tons).
- The calculated value is populated in the Nominal Capacity (Tons) field.

No validation errors are shown for leaving Nominal Capacity (Tons) empty prior to calculation.

The model can be saved successfully


TMD-26579 Verify auto-calculation of Nominal Capacity (kW) when Nominal Capacity (Tons) is entered first

## Test step
1. Locate the Nominal Capacity (kW) field.
2. Verify that the Nominal Capacity (kW) field is optional.
3. Leave the Nominal Capacity (kW) field empty.
4. Enter a valid numeric value in the Nominal Capacity (Tons) field.
5. Click outside the field or attempt to save the model.
6. Observe the Nominal Capacity (kW) field.
   1. kW to tons:   kW number / ( 12,000 X 0.0002930711 )
   2. tons to kW: tons number X 12,000 X 0.0002930711

## Test Result
The Nominal Capacity (kW) field is displayed and not marked as required.

When Nominal Capacity (Tons) is entered first:
- The system automatically calculates the corresponding Nominal Capacity (kW) value.
- The calculated value is populated in the Nominal Capacity (kW) field.

No validation errors are displayed.

The model can be saved successfully.