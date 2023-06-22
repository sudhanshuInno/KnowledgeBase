# **WEBHOOK FLOW:**
**STEP 1:**

- **Create Data model**



**STEP 2:**

- **Create collection(with properties in it)**



**(Note: In above example we are creating collection named ‘Contact’ and properties are ‘name', ‘phone’, ‘email’, 'created\_at’)**

**STEP 3:**

- **Navigate to ‘Webhook’ & select ‘Create Web Hook’**



**STEP 4:**

- **Create webhook with details:**
- **Example**
  - **Web Hook Name: ‘Get all collections’**
  - **URL: ‘/Contact’**
  - **Description: ‘Get all contacts’**
  - **Method: ‘GET’**

**CASE 1: Next step:**

**Select options as following**

- **DATABASE:** Get multi object and count by query 
- **Query String parameters:** Page, Size, Sort and Filters
- **OBJECT**: N/A
- **RESPONSE**: Return Success Response & Return Error Response**.**







- **CASE 2 - Example**
  - **Web Hook Name: ‘Post collections’**
  - **URL: ‘/Contact’**
  - **Description: ‘Post all collection’**
  - **Method: ‘POST’**

**Select options as following:**

- **DATABASE:** Create Single Object
- **LOGICAL:** N/A
- **OBJECT:** Get Object Value (Type ‘Body’ picked value option)
- **RESPONSE:** Return Success Response & Return Error Response.
- **First Select, ‘Get Object Value’ - add ‘body’ in ‘Picked Value’**



- **Second Select, ‘Create Single Object’, & choose collection name like we selected ‘contact’.**



**STEP 5:**

- **Both webhook made will be displayed on UI**



- **Deploy the created webhooks through Deploy BE(will ask for a password)**



- **Check the status of deployment from AWS as SUCCESS/FAIL.**
- **Go to API Docs section , Webhook endpoints will be reflected along with Base URL value.**



- **Click on “Get” then on “Try it Out” and then click on “Execute it”. It will get the records saved in collection.**



- **To POST the data in the collection, go to POST then click on “Try it out” and provide the data you want to save and then click on “Execute it”.**



- **After adding data through POST then click on “Data” section and then newly added data will be reflected in that particular Collection(here contacts)**



- **Here is the doc link for the APIs available**

<https://docs.google.com/spreadsheets/d/1Lmdc6uM59ENd5QMJzTz9ME6JgJ4loi1LmM0k14O2ZxI/edit?usp=sharing>
