# **Run Javascript Node**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure.



- Now drag Get single record by id node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add record id.

**IMPORTANT: ( input.[params.id](http://params.id/) is used as record id value to get the id from params ).**



- Now drag Get Aggregate results by grouping node, connect edge between request and input handles.
- Select a collection from grouped record model dropdown.
- Add expression in the select query field in case the user want to extract only those records that fulfill the specified expression. **(Optional)**



- Now drag Run Javascript Code node, connect edge multiple output request handles.
- Write your javascript logic in Javascript code field & you can access input from other node by using **ctx.InputEdgeHandleName** (i.e found & output in below example)



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.


