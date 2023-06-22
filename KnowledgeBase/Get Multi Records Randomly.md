# **Get Multi Records Randomly**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/8bc3856e-c72c-4a2e-8b49-884351267c19)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/afd5e710-dc17-4a27-a8d3-e99cd2b1cf41)



- Now drag Get multi records randomly node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add size to set how many records to show.

**( Possible value of size can be :** 

- any number, in this the the number of displayed records will be the provided number.
- ‘params.query.size’ , in this case the records will be displayed according to the value provided in params.
- null, in this case the records will be displayed according to the default value i.e. 10.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/44be0056-f3b9-435e-a606-c49b43af80d7)

- Add return error response and return success response nodes, connect edge between output and trigger handles of error response node to get error messages in case the request fails.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b96070f9-10d4-4337-bc81-bd8ab562c05c)



- Connect edge between trigger and output handles of success response to get success message and another edge to get the response in case the request is successful.

**IMPORTANT: (Another edge is required in case the user wants the response of the request)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/f40319a5-500a-41dd-a216-e261fd10bd60)



- This is all a user have to do to create the ‘get multi records randomly’ method.
