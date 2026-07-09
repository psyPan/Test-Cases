TMD-26484 Airflow Rate Default and Validation
## Test Steps
1. Create a Heat Rejection item from a model with Airflow Rate
2. Review that Airflow is added to the item

1. Create a Heat Rejection item from a model without Airflow Rate
2. Review Airflow value

## Test Results
1. Verify If model has Airflow Rate, item inherits the value from the model value
2. Airflow Rate field is optional