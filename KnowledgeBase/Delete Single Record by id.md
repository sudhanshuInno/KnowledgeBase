# **Delete Single Record by id**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure.



- Now drag delete single record by id node, connect edge between request and input handles.
- Select a collection from deleted record model dropdown and add id of the record to be deleted.

Add return error response and return success response nodes, connect edge between success and trigger handles of error response node to get error messages in case the request fails.



- Connect edge between trigger and success handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**



- This is all a user have to do to create the ‘delete single record by id’ method.
