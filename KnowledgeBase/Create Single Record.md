# **Create Single Record**
- Enter the webhook name, URL, and description, and choose the appropriate method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b40cda3c-ce52-4a41-abc5-ac1dbde39ed9)



- Click on the edit button to create webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/6e879d9e-d370-43d8-8fad-5e84fab4b17c)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/934b7ddd-2374-47cf-a154-ff3e1e81478a)

- Now drag Get Record Value node, add body in the picked value and connect edge between request and input handles.

**IMPORTANT:** ( Get Record Value node is required in case of creating and updating records to pass the body )
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/250189ae-0466-42bd-b658-6e529a748b8e)

- Now drag Create Single record node.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/7df84420-f68f-4530-a9d6-8aa93b082753)



- Connect edge between pickedValue and input handles.
- Select a collection from created record model dropdown.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/aead5959-248c-428e-afd3-52c00c89c0e0)



- Add return error response and return success response nodes, connect edge between created and trigger handles of error response node to get error messages in case the request fails.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/227b616d-2be2-46ff-8e33-bee1b40ce0be)



- Connect edge between trigger and created handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/1a4a1230-084f-49cf-a215-54ddd5e9fef3)



- This is all a user have to do to create the ‘create single record’ method.
