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

3. open the postman make requets such as :
     1.set GET and send http://localhost:3000/api/data  => this fetches all the data
     2.set GET and send http://localhost:3000/api/data/124 => this fetches data with id 124 (can change acordingly)
     3.set GET and send http://localhost:3000/api/data/assign/John Smith => this fetches data with assignee John Smith (first 10 tasks by an assignee, sorted by startTime) (can change acordingly)
     4.set GET and send http://localhost:3000/api/data/names/=> fetches based on names 
     5.set post and send http://localhost:3000/api/data with data in the body 
{
    "name": "install linux",
    "id": "124",
    "assignee": "John Smith",
    "project": "Kaiburr",
    "startTime": "2023-04-21 15:51:42.276Z"
}
 => creates new data 

    6.set delete and http://localhost:3000/api/data/124 => to delete for given id 124 
