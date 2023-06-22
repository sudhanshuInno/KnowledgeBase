# **SQL Expression Node**
**SELECT QUERY**

- Created a webhook using name, URL, description, and method type



- Start node is added by default and select the body type to none and save it.



- Add node of SQL Query and connect it from the start node.



- Add sql expression in the field by clicking on the expression model and add select query
- query added is “SELECT \* FROM $users$;“
- Make sure that sql keywords must in uppercase and model name must enclosed by dollar sign.



- Add 'return success response' node and connect it from sql query with trigger and extra handle for output.



- Added 'return error response' node in case of any error occurs.



- Output result when Endpoint is executed.



**GET SELECTED FIELDS**

- Create a webhook for getting selected field of table by passing name, URL, description, method.



- By default start node is added and selected body of type single and save it.



- Added ‘get record value' node to get the value and passing “input.body” in the picked Value and connect it from start node.



- Added 'sql expression node' and connect it to get record value.



- Added query “SELECT users.first\_name, users.last\_name FROM $users$ WHERE users.id = {{input.uid}};“
- Make sure that sql keywords must in uppercase and model name must enclosed by dollar sign.



- Added “return success response” and “return error response” and connect it from the “sql query” node
  and added extra edge in success response to get output.



**CREATE USER**

- Added webhook method for creating new user and passed name, URL, description, method. 



- Added body in start node and save it.



- Added ‘get record value' node and added 'input.body’ in picked value and connect it from start node.



- Added sql query node and connect it from get record value node.



- Added sql query “INSERT INTO $users$ (first\_name,id) VALUES ({{input.fname}},{{input.uid}});“.
- If using dynamic values must enclosed with double curly brackets.
- Make sure that sql keywords must in uppercase and model name must enclosed by dollar sign.
- Validated it after adding query.



- Added “return success response“ and “return error response“ and connect it to sql query.



- Output data after executing the service.



**UPDATE USER**

- Added body in start node and save it. 



- Added ‘get record value' node and added 'input.body’ in picked value and connect it from start node.
- Added 'sql expression node' and connect it to get record value.



- Added sql query “UPDATE $users$ SET first\_name = {{input.fname}}, last\_name = {{input.lname}} WHERE id = {{input.uid}};“.
- If using dynamic values must enclosed with double curly brackets.
- Make sure that sql keywords must in uppercase and model name must enclosed by dollar sign.
- Validated it after adding query.



- Added “return success response“ and “return error response“ and connect it to sql query.



- Output after executing the service.



**DELETE QUERY**

- Create a webhook for getting Delete query table by passing name, URL, description, method.
- Added body and save the in start node.



- Added ‘get record value' node and added 'input.body’ in picked value and connect it from start node.



- Added 'sql expression node' and connect it to get record value.



- Added sql query “DELETE FROM $users$ WHERE id={{input.uid}};“.
- If using dynamic values must enclosed with double curly brackets.
- Make sure that sql keywords must in uppercase and model name must enclosed by dollar sign.
- Validated it after adding query.



- Added “return success response“ and “return error response“ and connect it to sql query.



- Output after executing the services.


