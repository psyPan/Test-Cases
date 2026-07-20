TMD-26509 Verify the Potential Power field in Cooling Unit Models
## Test Steps
Create a Cooling Unit Model and add power ports to it. Verify that there is a field Potential Power, that is the sum of all non-redundant ports Budget Watts.

## Test Results
The field is only in the Model List, not in the details page. It displays the correct value.
There is no field Effective Power.

TMD-26630 Verify Fluid Flow Rate values in Cooling Unit.
## Test Steps
1. Create a Cooling Unit Model. Verify it has a field Fluid Flow Rate which is below the Airflow Rate in the Configuration (Should be Specification) sub-tab. Add a value. Create an Item – the field should be there and filled with the seed value from the model. Edit the value. Save.

2. In Models and Items test with values of 7 digits, 5 digits after the comma, negative numbers – they should not be accepted, because the variable in the DB is decimal (10,4). Empty value should be OK.

3. Test the conversion between Gallons and Liters when the Unit system is changed between US and SI (for instance 22 gallons should be about 83 liters)

## Test Results
The Fluid Flow Rate field is present and its initial value in the Item is determined by the model. The values are correct.