# **Get Multi Records Randomly**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure.



- Now drag Get multi records randomly node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add size to set how many records to show.

**( Possible value of size can be :** 

- any number, in this the the number of displayed records will be the provided number.
- ‘params.query.size’ , in this case the records will be displayed according to the value provided in params.
- null, in this case the records will be displayed according to the default value i.e. 10.

Add return error response and return success response nodes, connect edge between output and trigger handles of error response node to get error messages in case the request fails.



- Connect edge between trigger and output handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**



- This is all a user have to do to create the ‘get multi records randomly’ method.
