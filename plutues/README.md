
# Plutus-by-Unicohub-backend-assesment
<h1>Explanation</h1>
NodeJS Server with Express and MongoDB
This is a NodeJS server built using the Express framework and connected to a locally hosted MongoDB database. The server provides REST APIs for creating and retrieving users, posts, and likes, as well as a "famous" endpoint that returns the top 10 most liked posts. The server also includes functionality to send an email to the creator of a post if it becomes "famous".

<h1>Requirements</h1>
NodeJS (v14 or higher)
MongoDB
Nodemailer (for sending emails)
Installation
Clone the repository: git clone https://github.com/Pradyumancoder/Plutus-by-Unicohub-backend-assesment

Install dependencies: npm install

Set environment variables in a .env file in the root directory of the project:

makefile
Copy code
PORT=3000
DB_URL=mongodb://localhost:27017/my-database
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_SERVICE=gmail
SMTP_MAIL=youremail@gmail.com
SMTP_PASSWORD=yourpassword
Start the server: npm start

API Endpoints

Creates a new user in the database.
File Structure
![Screenshot_20230217_143824](https://user-images.githubusercontent.com/97114184/219614870-94218ba8-e9d9-47df-bc2f-130f2f832c2a.png)[code-structure]

POST /user
![Screenshot (7)](https://user-images.githubusercontent.com/97114184/219617523-db9d7737-33a2-4e7e-8036-f8396bc44fd2.png)[post/user]

GET /user
![Screenshot (11)](https://user-images.githubusercontent.com/97114184/219614864-55036536-cff9-4944-8d23-5c968cc8dd83.png)[get/user]

Returns information about the current user.

Response:
POST /post
![Screenshot (7)](https://user-images.githubusercontent.com/97114184/219614847-0f0c4e1e-3635-48c2-b59a-9adc9be9d30f.png)[post/post]


GET /post
![Screenshot (8)](https://user-images.githubusercontent.com/97114184/219614851-b90a5c6e-4d98-445f-b9e8-9c711813eec6.png)[get/post]

Returns all posts saved in the database, along with the number of likes for each post.
Response:

POST/likes
![Screenshot (9)](https://user-images.githubusercontent.com/97114184/219614854-d652b35e-d1c7-4293-9b99-2ea3676be734.png)[post/likes]


GET/famous
![Screenshot (10)](https://user-images.githubusercontent.com/97114184/219614859-5cf4bef1-3483-4bf5-91c5-f20a8c2602f5.png)[get/famous]

Email-sent
![Screenshot_20230217_153156](https://user-images.githubusercontent.com/97114184/219614875-1376cc3c-e52d-4cec-8c34-9f93222c1091.png)[sent-email]


