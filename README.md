# Digital Verification System

This project is a digital verification system for university certifications and transcripts, allowing students and employers to authenticate academic records online. The system is built using React.js for the frontend and Node.js with Express.js for the backend.
### Features

    User Authentication: Secure login and registration using JWT.
    Transcript Management: Upload, manage, and view transcripts.
    Verification: Employers can verify the authenticity of transcripts using student ID and name.

### Technology Stack

    Frontend: React.js
    Backend: Node.js, Express.js
    Database: Mysql (or PostgreSQL)
    Authentication: JWT (JSON Web Tokens)

### Prerequisites

    Node.js (v14.x or later)
    MongoDB (if using PostgreSQL, adjust instructions accordingly)
    npm or yarn

### Installation
## Backend

    Clone the repository:

    sh

git clone https://github.com/yourusername/digital-verification-system.git
cd digital-verification-system/backend

Install dependencies:

sh

npm install

Create a .env file in the backend directory and add the following:

env

PORT=3000
MONGO_URI=mongodb://localhost:27017/digital_verification
JWT_SECRET=your_jwt_secret

Start the backend server:

sh

    npm start

## Frontend

    Navigate to the frontend directory:

    sh

cd ../frontend

Install dependencies:

sh

npm install

Create a .env file in the frontend directory and add the following:

env

REACT_APP_API_URL=http://localhost:3000

Start the frontend development server:

sh

    npm start

Usage

    Open your browser and navigate to http://localhost:3000.
    Register a new user account.
    Log in with your credentials.
    Upload transcripts through the admin panel.
    View and verify transcripts using the provided student ID and name.

### API Endpoints
### Authentication

    POST /register: Register a new user
    POST /login: Log in an existing user

### Transcripts

    GET /transcript/:id: Get a transcript by ID
    POST /transcript: Add a new transcript (admin only)
