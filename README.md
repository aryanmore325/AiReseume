ResumeXpert API (CRUD App)

Overview

The ResumeXpert API is a simple CRUD (Create, Read, Update, Delete) application that allows users to manage their resumes. This API is built using Node.js, Express.js, and MongoDB.

LIVE URL

ai-reseume-nsfmo39bw-aryanmore325s-projects.vercel.app

Features

Create a new resume

Retrieve all resumes

Retrieve a specific resume by ID

Update a resume by ID

Delete a resume by ID

Technologies Used

Node.js

Express.js

MongoDB (Mongoose ODM)

Postman (for testing API endpoints)

Installation

Clone the repository:

git clone https://github.com/your-username/resumeXpert-api.git

Navigate to the project directory:

cd resumeXpert-api

Install dependencies:

npm install

Set up environment variables:

Create a .env file in the root directory and add the following:

PORT=5000
MONGO_URI=your_mongodb_connection_string

Start the server:

npm start

API Endpoints

1. Create a Resume

Endpoint: POST /api/resumes

Description: Creates a new resume.

Request Body:

{
  "name": "John Doe",
  "email": "johndoe@example.com",
  "phone": "123-456-7890",
  "skills": ["JavaScript", "React", "Node.js"],
  "experience": [
    {
      "company": "Tech Corp",
      "role": "Software Engineer",
      "years": 2
    }
  ]
}

Response:

{
  "_id": "resume_id",
  "name": "John Doe",
  "email": "johndoe@example.com",
  "phone": "123-456-7890",
  "skills": ["JavaScript", "React", "Node.js"],
  "experience": [
    {
      "company": "Tech Corp",
      "role": "Software Engineer",
      "years": 2
    }
  ],
  "createdAt": "timestamp",
  "updatedAt": "timestamp"
}

2. Get All Resumes

Endpoint: GET /api/resumes

Description: Retrieves all resumes.

Response:

[
  {
    "_id": "resume_id",
    "name": "John Doe",
    "email": "johndoe@example.com"
  }
]

3. Get a Resume by ID

Endpoint: GET /api/resumes/:id

Description: Retrieves a specific resume by ID.

4. Update a Resume

Endpoint: PUT /api/resumes/:id

Description: Updates a resume by ID.

Request Body:

{
  "name": "John Doe Updated",
  "skills": ["JavaScript", "React", "TypeScript"]
}

5. Delete a Resume

Endpoint: DELETE /api/resumes/:id

Description: Deletes a resume by ID.

Database Schema

Collections and Relationships:

resumes: Stores the resumes created by users.

users: Stores user profile information such as name, email, and phone.

skills: Stores skill tags that users can associate with their resumes.

experience: Stores work experience details, including company name, role, and years worked.

License

This project is licensed under the MIT License.

Author

Created by Aryan Morre & John Doe.

