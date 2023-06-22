# **Get Multi Records And Count By Query**
- Enter the webhook name, URL, and description, and choose the appropriate method. After the webhook is created click on the edit button to create the webhook method.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/79fd4073-5ccf-410c-a383-4eb8cff4a2ed)

- Create query parameters for page, size & sort
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/5a698e23-63d5-47de-ab38-1ca187e31c75)



- Now drag Get multi records and count by query node, connect edge between request and input handles.
- Select a collection from retrieved record model dropdown and add size, page & sort to set how many records to show & in what manner.

**( Possible value of size & page can be :**

- any number, in this the the number of displayed records will be the provided number.
- ‘params.query.size’ , in this case the records will be displayed according to the value provided in params.
- null, in this case the records will be displayed according to the default value i.e. 10.

**)**

- **( Possible value of sort :**
  - text in form of “[columnName: asc/desc, columnName: asc/desc,…]”

**)**
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/076a9c30-139d-428b-b250-11ed83f0d356)
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/052d381a-c972-4404-9d79-83ead4e582b0)

- Add return error response and return success response nodes, connect edge between output and trigger handles of error response node to get error messages in case the request fails.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/e5cd4fa9-a787-495c-a145-54d9a011f249)



**IMPORTANT: (Another edge is required in case the user wants the response of the request with countInfo)**

Example:-
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/1f74013b-16da-4ff7-a3f4-d048eb03fb0b)

