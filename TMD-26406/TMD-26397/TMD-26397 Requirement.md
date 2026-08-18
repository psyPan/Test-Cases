TMD-26397 Check the manifold subclass in various screens
## Test Steps
1. In the Manifold item details, add it to a project. Edit a Project to add a new Manifold item. Both items should be visible in the Project-Items subtab.

2. In a Circuit trace of an existing Circuit and when creating a new Circuit, verify that the item selection grid has HVAC/Manifold in the subclass dropdown.

3. In a Ticket, Items tab, assign a Manifold item by selecting class and subclass.

4. In the Data Network Diagram, verify that the item selection grid has HVAC/Manifold in the subclass dropdown.

5. Create a new Custom Field and assign it to Items of Class HVAC, subclass Manifold. Create another, that is applicable to all classes. Add it to Design Subtab and verify that it is visible in the Item Details page. While there check that the filter on the left and the Identify button is working for HVAC/Manifold

6. Create a Custom Field for the Models of subclass Manifold.

## Test Results
1. Successful selection of the class and subclass of Manifold