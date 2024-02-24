**Project: OneServer - Realtime Data Sharing**

**Developed by: Subham Mandal**

use : https://cdn.jsdelivr.net/gh/Subham-Mandal/oneserver@master/code.js
---

**Introduction:**

OneServer is a real-time data sharing platform developed by Subham Mandal. This platform facilitates seamless exchange of data among users using Firebase Database Functions. With OneServer, users can easily share and retrieve data in real-time, enabling efficient collaboration and communication.

---


**Instructions:**

1. **LOAD Function:**

   - **Function Syntax:** `LOAD(path, callback)`

   - **Purpose:** Loads data from the specified path in the Firebase database.

   - **Parameters:**
     - `path`: The path in the database from which to load data.
     - `callback`: A function to handle the loaded data.

   - **Usage Example:**
     ```javascript
     LOAD("path/to/data", function(data) {
         // Handle loaded data here
     });
     ```

2. **GET Function:**

   - **Function Syntax:** `GET(path, callback)`

   - **Purpose:** Retrieves the last value from the specified path in the Firebase database.

   - **Parameters:**
     - `path`: The path in the database from which to retrieve data.
     - `callback`: A function to handle the retrieved data.

   - **Usage Example:**
     ```javascript
     GET("path/to/data", function(data) {
         // Handle retrieved data here
     });
     ```

3. **PUSH Function:**

   - **Function Syntax:** `PUSH(path, text, successCallback, errorCallback)`

   - **Purpose:** Pushes data to the specified path in the Firebase database.

   - **Parameters:**
     - `path`: The path in the database to which data will be pushed.
     - `text`: The data to be pushed.
     - `successCallback`: (Optional) A function to execute on successful data push.
     - `errorCallback`: (Optional) A function to execute on error during data push.

   - **Usage Example:**
     ```javascript
     PUSH("path/to/data", "Data to push", 
         function(successMessage) {
             // Handle success
         },
         function(errorMessage) {
             // Handle error
         });
     ```

4. **SET Function:**

   - **Function Syntax:** `SET(path, text, successCallback, errorCallback)`

   - **Purpose:** Sets data at the specified path in the Firebase database.

   - **Parameters:**
     - `path`: The path in the database where data will be set.
     - `text`: The data to be set.
     - `successCallback`: (Optional) A function to execute on successful data set.
     - `errorCallback`: (Optional) A function to execute on error during data set.

   - **Usage Example:**
     ```javascript
     SET("path/to/data", "Data to set", 
         function(successMessage) {
             // Handle success
         },
         function(errorMessage) {
             // Handle error
         });
     ```

5. **DEPLOY Function:**

**NEW UPDATE : use EVENT(functionName,path) instead of DEPLOY for store message (PUSH-GET) system**

   - **Function Syntax:** `DEPLOY(myFunction, path, key)`

   - **Purpose:** Deploys a function to run whenever data changes at the specified path in the Firebase database.

   - **Parameters:**
     - `myFunction`: The function to be deployed.
     - `path`: The path in the database to monitor for changes.
     - `key`: The key associated with the path.

   - **Usage Example:**
     ```javascript
     DEPLOY(myFunction, "path/to/data", "key",
         function(data) {
             // Function to execute on data change
         });
     ```

6. **DELETE Function:**

   - **Function Syntax:** `DELETE(path, text, successCallback, errorCallback)`

   - **Purpose:** Deletes data from the specified path in the Firebase database.

   - **Parameters:**
     - `path`: The path in the database from which data will be deleted.
     - `text`: (Optional) The specific data to be deleted.
     - `successCallback`: (Optional) A function to execute on successful data deletion.
     - `errorCallback`: (Optional) A function to execute on error during data deletion.

   - **Usage Example:**
     ```javascript
     DELETE("path/to/data", "Data to delete", 
         function(successMessage) {
             // Handle success
         },
         function(errorMessage) {
             // Handle error
         });
     ```

---

**Conclusion:**

With OneServer, Subham Mandal has developed a powerful real-time data sharing platform, offering efficient collaboration and communication among users. Whether you're loading existing data, pushing new updates, or deploying custom functions, OneServer provides a seamless solution for real-time data exchange.

For more information and support, refer to the documentation or contact Subham Mandal.

---

