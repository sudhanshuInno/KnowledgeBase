# **Get Single Record by id**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/1a42f352-fcda-4b3f-be4c-b3a63475dc90)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/6f35bdad-771f-4139-8aaf-5bc4adde986d)



- Now drag Get single record by id node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add record id.

**IMPORTANT: ( [params.id](http://params.id) is used as record id value to get the id from params ).**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/70f9a14f-23e4-4455-806c-3b097e1028af)

- Add return error response and return success response nodes, connect edge between not found and trigger handles of error response node to get error messages in case the request fails.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/66ef5662-eebb-4609-9cb6-90f708068352)



- Connect edge between trigger and found handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/2879f7e8-4463-48bc-8423-25327b9af79b)



- This is all a user have to do to create the ‘get single record by id’ method.
