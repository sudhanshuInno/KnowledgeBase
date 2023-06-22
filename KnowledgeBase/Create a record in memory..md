# **Create a record in memory.**
Create two collections like Users & Contacts, and also add userid one-to-many property in the Contacts collection.



Visit the webhook section and create a webhook with the following details.



Select multi in the body options and additional details for both collections.



Add two 'get record value' nodes and add the following details.



Add a 'Create Single Record' node and select the Users collection in it.



Add a ‘Create Record In Memory' node and join it with the ‘Create Single Record' node.



Select the Contacts collection in the 'Create Record In Memory' node.



Click on the ‘Manage Updates' button & select the 'userid’ option in the popped-up model.



Now click on the ‘fx' icon and select the 'id’ option from the created section.



Add a ‘Create Single Record' node and select the Contacts collection in it.



Add ‘Return Success Response' and 'Return Error Response’ and connect the edges as per the image.


