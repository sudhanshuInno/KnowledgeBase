# **Create Multi Records**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure.

Now drag Get Record Value node, add body in the picked value and connect edge between request and input handles.

**IMPORTANT:** ( Get Record Value node is required in case of creating and updating records to pass the body )

Now drag Create multi records node, connect edge between pickedValue and input handles.

- Select a collection from created records model dropdown.



- Add return error response and return success response nodes, connect edge between created and trigger handles of error response node to get error messages in case the request fails.



- Connect edge between trigger and created handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**



- This is all a user have to do to create the ‘create multi records’ method.
