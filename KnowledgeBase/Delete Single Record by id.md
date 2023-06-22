# **Delete Single Record by id**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/35227e0d-a50b-4b8b-8182-e5cc3d1ac663)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/a0a64bde-f759-4470-8061-1ef5c2f8f144)



- Now drag delete single record by id node, connect edge between request and input handles.
- Select a collection from deleted record model dropdown and add id of the record to be deleted.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/06a4ce00-0325-4201-b112-2c9d69b05901)

Add return error response and return success response nodes, connect edge between success and trigger handles of error response node to get error messages in case the request fails.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/fa5cc802-ae64-4fb5-80d7-9cc4f539fdc6)



- Connect edge between trigger and success handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/c89925e6-147c-4178-b70d-8dea91a543b2)



- This is all a user have to do to create the ‘delete single record by id’ method.
