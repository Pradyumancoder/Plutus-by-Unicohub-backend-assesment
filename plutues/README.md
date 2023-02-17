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
POST /user
Creates a new user in the database.

{
  "_id": "60b3c0ee3f9b9c3f3c3cb3d4",
  "name": "John Doe",
  "email": "johndoe@example.com",
  "password": "mypassword",
  "createdAt": "2021-05-30T20:50:54.468Z",
  "updatedAt": "2021-05-30T20:50:54.468Z",
  "__v": 0
}
GET /user
Returns information about the current user.

Response:

GET /post
Returns all posts saved in the database, along with the number of likes for each post.

Response: