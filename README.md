# ResumeXpert 

## Overview
The ResumeXpert is a simple application that allows users to manage their notes. This API is built using Node.js, Express.js, and MongoDB.

LIVE URL - ai-reseume.vercel.app

## Features
- Create a new note
- Retrieve all notes
- Retrieve a specific note by ID
- Update a note by ID
- Delete a note by ID

## Technologies Used
- Node.js
- Express.js
- MongoDB (with Mongoose ODM)
- Postman (for testing API endpoints)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/resumeXpert-api.git
   ```
2. Navigate to the project directory:
   ```bash
   cd resumeXpert-api
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add the following environment variables:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     ```
5. Start the server:
   ```bash
   npm start
   ```



## Database Schema
Database Schema

Below is the database schema used for the ResumeXpert API:

Collections and Relationships:

resumes: Stores the resumes created by users.

users: Stores user profile information such as name, email, and phone.

skills: Stores skill tags that users can associate with their resumes.

experience: Stores work experience details, including company name, role, and years worked.



## License
This project is licensed under the MIT License.

## Author
Created by ARYAN MORE .

