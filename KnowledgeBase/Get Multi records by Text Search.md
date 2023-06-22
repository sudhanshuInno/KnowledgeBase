# **Get Multi records by Text Search**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.



- Select the request body structure and create required query parameters.



- Now drag Get multi records by text search node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown.
- Add value of the search text field.
- **( Appropriate value of text search field should be:**
  - [column name: text to be searched]. (e.g. [columns.name](http://columns.name):”test”)

**)**



- Toggle return count info button to get the count info in success response.



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.
- Connect “countInfo” handle of Get multi records by text search with Return success response node to get the count Info in response.



- This is all a user have to do to create the ‘ Get multi records by text search’ method.

**RESULT:**


