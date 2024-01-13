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
![image](https://github.com/sri6703/task1/assets/113595807/1f01fdd9-787c-4329-ae40-9df084e3fedb)
![image](https://github.com/sri6703/task1/assets/113595807/ac53016a-4fb0-45f4-84cf-6f5ef92be58b)


2. **Fetch Data by ID:**
   - Set `GET` and send request to: `http://localhost:3000/api/data/124`
   - This fetches data with ID 124 (change the ID accordingly).
   - ![image](https://github.com/sri6703/task1/assets/113595807/640f9256-49f7-4b5a-a33d-2a0a993619fe)
   - ![image](https://github.com/sri6703/task1/assets/113595807/61993e33-1511-4bd8-9110-904ce5a11cb7)
   - ![image](https://github.com/sri6703/task1/assets/113595807/be7baf72-a7e1-45c6-8aad-a04d59f46d34)

3. **Fetch Data by Assignee:**
   - Set `GET` and send request to: `http://localhost:3000/api/data/assign/John Smith`
   - This fetches data assigned to John Smith (first 10 tasks, sorted by startTime).
![image](https://github.com/sri6703/task1/assets/113595807/2611f07f-df9e-4e1f-86e6-b342e49b50de)
![image](https://github.com/sri6703/task1/assets/113595807/764cb808-2224-46eb-9e68-d6befcadf95d)


4. **Fetch Data by Name:**
   - Set `GET` and send request to: `http://localhost:3000/api/data/names/`
   - Fetches data based on names.
   - ![image](https://github.com/sri6703/task1/assets/113595807/df828718-b7f5-4e4d-9ae0-cf0271de7aa0)
   - ![image](https://github.com/sri6703/task1/assets/113595807/1416614d-be06-4f07-a30e-8459bfce837f)



5. **Create New Data:**
   - Set `POST` and send request to: `http://localhost:3000/api/data` with the following data in the body:
     ```json
{
    "name": "punitha",
    "id": "132",
    "assignee": "John Smith",
    "project": "Kaiburr",
    "startTime": "2023-04-21 15:51:42.276Z"
}
     ```
     This creates new data.
     ![image](https://github.com/sri6703/task1/assets/113595807/71b7beef-f2d4-426d-b6ce-04eeafe10a81)
     ![image](https://github.com/sri6703/task1/assets/113595807/fcdea201-47fd-46a4-b518-029816ae72bf)

6. **Delete Data by ID:**
   - Set `DELETE` and send request to: `http://localhost:3000/api/data/124`
   - Deletes data with the given ID (change the ID accordingly).
   - ![image](https://github.com/sri6703/task1/assets/113595807/456c394c-0fc2-4fcc-b8be-431ee10f7204)
   - ![image](https://github.com/sri6703/task1/assets/113595807/6edf889f-5237-4a2f-b24b-c133f6316c3a)


   


PHOTOS :


