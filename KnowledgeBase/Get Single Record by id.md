# **Get Single Record by id**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure.



- Now drag Get single record by id node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add record id.

**IMPORTANT: ( [params.id](http://params.id) is used as record id value to get the id from params ).**

Add return error response and return success response nodes, connect edge between not found and trigger handles of error response node to get error messages in case the request fails.



- Connect edge between trigger and found handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**



- This is all a user have to do to create the ‘get single record by id’ method.
