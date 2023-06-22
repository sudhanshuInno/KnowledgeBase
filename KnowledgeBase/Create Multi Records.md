# **Create Multi Records**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/59c76669-6e9a-41be-9ce4-59f1657fa76e)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/33289ef6-06b5-44e9-bff6-4b14ad0375a9)

- Now drag Get Record Value node, add body in the picked value and connect edge between request and input handles.

**IMPORTANT:** ( Get Record Value node is required in case of creating and updating records to pass the body )
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/aeb4dd81-eb3a-4ce7-9c5f-aa17971ee03a)

- Now drag Create multi records node, connect edge between pickedValue and input handles.

- Select a collection from created records model dropdown.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/0838618f-393b-4dff-8f15-84ec6addf783)



- Add return error response and return success response nodes, connect edge between created and trigger handles of error response node to get error messages in case the request fails.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/64a4c3c7-b45a-4b55-8e56-c92aa6e8b68d)



- Connect edge between trigger and created handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/c8220c70-c91c-478d-b2fe-4600f3c45f9e)



- This is all a user have to do to create the ‘create multi records’ method.
