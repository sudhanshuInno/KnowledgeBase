# **Get Aggregate Results by Grouping**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure.



- Now drag Get Aggregate results by grouping node, connect edge between request and input handles.
- Select a collection from grouped record model dropdown.
- Add expression in the select query field in case the user want to extract only those records that fulfill the specified expression. **(Optional)**



- Select the value of the group by field.

**NOTE: Group by field specifies how the user want to group the result.**



- Now add computations by clicking the add computation button.
- Select name, sort order and type of the computation field and hit save button.



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**



- This is all a user have to do to create the ‘Get aggregate results by grouping’ method.

**RESULT:** 

