TMD-26400 Test subclass change in existing Manifold model
## Test Steps
1. In Models Library, change the subclass of the existing model to another in class HVAC, like “Cooling Unit”. Create a new Cooling Unit and change its subclass to Manifold and back again

## Test Results
1. Error on the existing model – there are items using it. With the new model, re-assignment is possible.