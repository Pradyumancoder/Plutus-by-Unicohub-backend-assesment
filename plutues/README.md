![Screenshot (1)](https://user-images.githubusercontent.com/97114184/219614796-63fcbe80-c00a-4fc6-a492-bcbd16b0cbef.png)
![Screenshot (2)](https://user-images.githubusercontent.com/97114184/219614821-a2fe4ac6-5f3d-41fa-b385-9aecec1f4edd.png)
![Screenshot (3)](https://user-images.githubusercontent.com/97114184/219614829-eddfd2c2-5417-429c-b1d3-eeed36a1cbc8.png)
![Screenshot (4)](https://user-images.githubusercontent.com/97114184/219614835-9dba667c-8812-40cc-af4c-11a83e07380e.png)
![Screenshot (5)](https://user-images.githubusercontent.com/97114184/219614842-feab18c5-b52c-45c6-a640-8438de9b5de3.png)
![Screenshot (6)](https://user-images.githubusercontent.com/97114184/219614845-3cdcf3f3-5450-4b07-9f72-4bba8adfda92.png)
![Screenshot (7)](https://user-images.githubusercontent.com/97114184/219614847-0f0c4e1e-3635-48c2-b59a-9adc9be9d30f.png)
![Screenshot (8)](https://user-images.githubusercontent.com/97114184/219614851-b90a5c6e-4d98-445f-b9e8-9c711813eec6.png)
![Screenshot (9)](https://user-images.githubusercontent.com/97114184/219614854-d652b35e-d1c7-4293-9b99-2ea3676be734.png)
![Screenshot (10)](https://user-images.githubusercontent.com/97114184/219614859-5cf4bef1-3483-4bf5-91c5-f20a8c2602f5.png)
![Screenshot (11)](https://user-images.githubusercontent.com/97114184/219614864-55036536-cff9-4944-8d23-5c968cc8dd83.png)
![Screenshot_20230217_143824](https://user-images.githubusercontent.com/97114184/219614870-94218ba8-e9d9-47df-bc2f-130f2f832c2a.png)
![Screenshot_20230217_153139](https://user-images.githubusercontent.com/97114184/219614872-d765b9c5-f9bb-4a86-ab55-9da68924d500.png)
![Screenshot_20230217_153156](https://user-images.githubusercontent.com/97114184/219614875-1376cc3c-e52d-4cec-8c34-9f93222c1091.png)
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


GET /user
Returns information about the current user.

Response:
POST /post

GET /post

Returns all posts saved in the database, along with the number of likes for each post.
Response:

POST/likes


GET/famous


