# **Run Javascript Node**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b4810b9c-b92d-479f-80af-771dc541bb3d)



- Select the request body structure.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/fa98ce39-7a48-4faa-8e38-22b91d39fe4d)



- Now drag Get single record by id node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add record id.

**IMPORTANT: ( input.[params.id](http://params.id/) is used as record id value to get the id from params ).**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/6d5539ef-8b9d-4c0f-9e93-60d1eb32fcdc)



- Now drag Get Aggregate results by grouping node, connect edge between request and input handles.
- Select a collection from grouped record model dropdown.
- Add expression in the select query field in case the user want to extract only those records that fulfill the specified expression. **(Optional)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b4162833-df1f-46dc-9283-619b0ea572c8)



- Now drag Run Javascript Code node, connect edge multiple output request handles.
- Write your javascript logic in Javascript code field & you can access input from other node by using **ctx.InputEdgeHandleName** (i.e found & output in below example)
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/086d69f1-7500-4341-88ae-efb3f51ef527)



- Add return error response and return success response nodes, connect edge between result and trigger handles of error response node to get error messages in case the request fails.
- Connect edge between trigger and result handles of success response to get success message and another edge to get the response in case the request is successful.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/d77d1bbe-0728-4cfc-8fb5-cc489fbe03f0)


