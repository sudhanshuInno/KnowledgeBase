# **Get Aggregate Results by Grouping**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/f9b94449-ad2b-4492-b792-2865e89b1289)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/f18456cf-5199-4844-8007-7e0cff4a9b8c)



- Now drag Get Aggregate results by grouping node, connect edge between request and input handles.
- Select a collection from grouped record model dropdown.
- Add expression in the select query field in case the user want to extract only those records that fulfill the specified expression. **(Optional)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/d46eb3c8-3645-45ef-a3ca-d6a917ee745f)



- Select the value of the group by field.

**NOTE: Group by field specifies how the user want to group the result.**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/4d54384e-ef40-4775-b1e7-179a793528d5)



- Now add computations by clicking the add computation button.
- Select name, sort order and type of the computation field and hit save button.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/31a36bf6-c9e1-4428-abf8-404a6b452c69)



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b8c4d379-3a91-4cb0-8a2c-85983afe8c62)



- This is all a user have to do to create the ‘Get aggregate results by grouping’ method.

**RESULT:** 
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/c6d9596f-0598-40cf-96c1-712a9fb235aa)

