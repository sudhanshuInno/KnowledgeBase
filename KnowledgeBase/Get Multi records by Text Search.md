# **Get Multi records by Text Search**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/d734e2bc-5704-47d0-8273-dbe918e5fcb8)



- Select the request body structure and create required query parameters.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b2b3f4ee-8063-44c0-83fb-f86afc23f4f1)



- Now drag Get multi records by text search node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown.
- Add value of the search text field.
- **( Appropriate value of text search field should be:**
  - [column name: text to be searched]. (e.g. [columns.name](http://columns.name):”test”)

**)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/7a366ff3-a37e-47cb-9fed-f07106444e61)



- Toggle return count info button to get the count info in success response.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/8747660f-91c5-443f-90ea-b207912f6838)



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.
- Connect “countInfo” handle of Get multi records by text search with Return success response node to get the count Info in response.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/0af14153-9981-4ce0-a33d-e00e63d6d808)



- This is all a user have to do to create the ‘ Get multi records by text search’ method.

**RESULT:**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/ed9eeb06-fecf-49b1-87f8-a6137dbc2608)


