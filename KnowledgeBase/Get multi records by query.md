# **Get multi records by query**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure and create required query parameters.



- Now drag Get multi records by query node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown.
- Add expression in the select query field in case the user want to extract only those records that fulfill the specified expression. **(Optional)**



- Now add value of the sort expression field.
- **( Possible values of sort expression field can be:**
  - text in form of “[columnName: asc/desc, columnName: asc/desc,…]”
  - params.query.sort , in this case the records will be displayed according to the value provided in params. (e.g. URL: [http://localhost:4001/users/query?sort=\[name:asc,phone:desc\]](http://localhost:4001/users/query?asc=[name:ASC,phone:DESC]))

**)**



- Toggle return count info button to get the count info in success response.



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.
- Connect “countInfo” handle of Get multi records by query with Return success response node to get the count Info in response.



- This is all a user have to do to create the ‘ Get multi records by query’ method.

**RESULT:**


