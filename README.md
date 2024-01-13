# task1
## Prerequisites

- Ensure you have MongoDB Compass installed and set up.
  1. Open MongoDB Compass.
  2. Create a new connection with the following address: `mongodb://127.0.0.1:27017`.
  3. Create a new database named `kaiburr`.
  4. Within the `kaiburr` database, create a collection named `model`.
  5. should have Postman to send requests .

## Getting Started

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/sri6703/task1.git
    ```
2. Opem a Terminal and run the following commands 

```bash
cd backend
npm install
node server.js
```
The backend server will run at http://localhost:3000.
## Testing API Endpoints with Postman

1. **Fetch All Data:**
   - Set `GET` and send request to: `http://localhost:3000/api/data`
   - This fetches all the data.

2. **Fetch Data by ID:**
   - Set `GET` and send request to: `http://localhost:3000/api/data/124`
   - This fetches data with ID 124 (change the ID accordingly).

3. **Fetch Data by Assignee:**
   - Set `GET` and send request to: `http://localhost:3000/api/data/assign/John Smith`
   - This fetches data assigned to John Smith (first 10 tasks, sorted by startTime).

4. **Fetch Data by Name:**
   - Set `GET` and send request to: `http://localhost:3000/api/data/names/`
   - Fetches data based on names.

5. **Create New Data:**
   - Set `POST` and send request to: `http://localhost:3000/api/data` with the following data in the body:
     ```json
     {
         "name": "install linux",
         "id": "124",
         "assignee": "John Smith",
         "project": "Kaiburr",
         "startTime": "2023-04-21 15:51:42.276Z"
     }
     ```
     This creates new data.

6. **Delete Data by ID:**
   - Set `DELETE` and send request to: `http://localhost:3000/api/data/124`
   - Deletes data with the given ID (change the ID accordingly).

