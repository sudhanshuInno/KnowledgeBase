# **Get multi records by query**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/0e5bec65-3405-4c4e-9bcd-12850ae43f75)



- Select the request body structure and create required query parameters.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/09296d35-31cf-45a7-9eed-7f5101a2a841)



- Now drag Get multi records by query node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown.
- Add expression in the select query field in case the user want to extract only those records that fulfill the specified expression. **(Optional)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/52b50180-0b55-4637-87f6-29313f19b378)



- Now add value of the sort expression field.
- **( Possible values of sort expression field can be:**
  - text in form of “[columnName: asc/desc, columnName: asc/desc,…]”
  - params.query.sort , in this case the records will be displayed according to the value provided in params. (e.g. URL: [http://localhost:4001/users/query?sort=\[name:asc,phone:desc\]](http://localhost:4001/users/query?asc=[name:ASC,phone:DESC]))

**)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/4db2c25e-7c67-4a46-9f8d-79c4772c283c)



- Toggle return count info button to get the count info in success response.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/71cb1d87-1d28-4495-a3c2-8fbe03c06427)



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.
- Connect “countInfo” handle of Get multi records by query with Return success response node to get the count Info in response.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/bd82b3ed-eb71-4922-81a5-3e082ab4af2b)



- This is all a user have to do to create the ‘ Get multi records by query’ method.

**RESULT:**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/60a3e4e5-12f7-4f12-b358-60fba492f284)


