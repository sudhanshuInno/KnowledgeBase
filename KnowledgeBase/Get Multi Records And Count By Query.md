# **Get Multi Records And Count By Query**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.

- Create query parameters for page, size & sort



- Now drag Get multi records and count by query node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add size, page & sort to set how many records to show & in what manner.

**( Possible value of size & page can be :**

- any number, in this the the number of displayed records will be the provided number.
- ‘params.query.size’ , in this case the records will be displayed according to the value provided in params.
- null, in this case the records will be displayed according to the default value i.e. 10.

**)**

- **( Possible value of sort :**
  - text in form of “[columnName: asc/desc, columnName: asc/desc,…]”

**)**

- Add return error response and return success response nodes, connect edge between output and trigger handles of error response node to get error messages in case the request fails.



**IMPORTANT: (Another edge is required in case the user wants the response of the request with countInfo)**

Example:-

