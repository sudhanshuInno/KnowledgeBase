# **Create a record in memory.**
Create two collections like Users & Contacts, and also add userid one-to-many property in the Contacts collection.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b172095c-08c4-4ac8-88ce-2e66374187cb)



Visit the webhook section and create a webhook with the following details.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/ae1e3c62-c270-4a13-a35d-50f5794b8f79)



Select multi in the body options and additional details for both collections.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/2f96a8d8-3456-4718-9337-2cbd9252f26a)



Add two 'get record value' nodes and add the following details.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/75eb2eb6-ee3b-429a-a725-ee79e56b52c9)
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/37c4898e-58f4-421b-a5ef-9252a2e11f81)



Add a 'Create Single Record' node and select the Users collection in it.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/09bf15a1-09a3-4678-8dd5-bdcb3ce0ac60)



Add a ‘Create Record In Memory' node and join it with the ‘Create Single Record' node.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/b7f93c1d-1e9b-4947-bca0-bbea22e38ac3)



Select the Contacts collection in the 'Create Record In Memory' node.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/db07a850-8ac0-43f4-8617-4beff7f1d5bd)



Click on the ‘Manage Updates' button & select the 'userid’ option in the popped-up model.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/8e463824-283e-4d9d-bf8d-728a74d4e902)



Now click on the ‘fx' icon and select the 'id’ option from the created section.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/51222a4e-b2ee-456c-95f9-9b9fd2f12a56)
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/65dbfe81-b04f-4aff-84a7-e973f883f3ea)
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/971365d0-908a-4a5b-9b9c-8721189c4d78)



Add a ‘Create Single Record' node and select the Contacts collection in it.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/4aa72b90-031a-4909-bba3-8bbf7297b513)



Add ‘Return Success Response' and 'Return Error Response’ and connect the edges as per the image.
![image](https://github.com/sudhanshuInno/KnowledgeBase/assets/126747849/80954b4a-3762-44db-a2d5-ec4055ee105a)


