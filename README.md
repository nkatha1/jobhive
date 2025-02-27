JobHive - Job Listing Platform
JobHive is a full-stack job listing platform where companies can post job openings, and candidates can view and apply for them. Built with a modern tech stack, JobHive provides an intuitive and scalable solution for job seekers and employers alike.

🚀 Features
Job Posting: Employers can easily create and post job opportunities.
Job Search: Candidates can search for jobs based on criteria like title, location, and salary.
Job Application: Candidates can apply to jobs with their profile.
User Authentication: Secure user login and registration for both candidates and employers.
Backend: Built with Node.js, Express.js, and MongoDB for a powerful, scalable backend.
Frontend: Designed with React to create a responsive and user-friendly interface.
💡 Technologies Used
Backend:

Node.js: A JavaScript runtime built on Chrome's V8 JavaScript engine.
Express.js: A minimal and flexible Node.js web application framework.
MongoDB: A NoSQL database used to store job postings, user data, and application details.
Mongoose: An ODM (Object Data Modeling) library for MongoDB and Node.js.
JWT (JSON Web Tokens): Used for user authentication.
Bcrypt.js: For securely hashing passwords.
Frontend:

React: A JavaScript library for building user interfaces.
Axios: A promise-based HTTP client for the browser and Node.js.
React Router: For navigation and routing in the frontend.
Material-UI: For pre-designed React components that provide a clean, modern UI.
🎯 Getting Started
Follow these steps to get the project up and running locally.

1. Clone the Repository
bash
Copy
git clone https://github.com/<your-username>/jobhive.git
cd jobhive
2. Install Backend Dependencies
Go to the backend directory and install the necessary dependencies.

bash
Copy
cd jobhive-backend
npm install
3. Configure .env for Backend
Create a .env file in the backend directory with the following environment variables:

bash
Copy
MONGO_URI=<Your MongoDB Atlas URI>
JWT_SECRET=<Your JWT secret key>
PORT=5000
Make sure to replace <Your MongoDB Atlas URI> with the connection string from your MongoDB Atlas cluster and <Your JWT secret key> with a strong secret key for encoding JWT tokens.

4. Install Frontend Dependencies
Go to the frontend directory and install the necessary dependencies.

bash
Copy
cd ../jobhive-frontend
npm install
5. Start the Backend Server
In the jobhive-backend directory, run the following command:

bash
Copy
npm run dev
This will start the backend server on http://localhost:5000.

6. Start the Frontend Server
In the jobhive-frontend directory, run the following command:

bash
Copy
npm start
This will start the frontend on http://localhost:3000.

🌐 API Endpoints
1. POST /api/jobs - Create a Job
Request Body:

json
Copy
{
  "title": "Software Engineer",
  "description": "Develop web applications.",
  "company": "Tech Corp",
  "location": "New York",
  "salary": 100000
}
Response:

json
Copy
{
  "message": "Job created successfully"
}
2. GET /api/jobs - Get All Jobs
Response:

json
Copy
[
  {
    "title": "Software Engineer",
    "company": "Tech Corp",
    "location": "New York",
    "salary": 100000
  },
  {
    "title": "Frontend Developer",
    "company": "Web Tech",
    "location": "San Francisco",
    "salary": 90000
  }
]
3. POST /api/users/register - Register a User
Request Body:

json
Copy
{
  "email": "user@example.com",
  "password": "yourpassword",
  "role": "candidate"
}
Response:

json
Copy
{
  "message": "User registered successfully"
}
4. POST /api/users/login - Login a User
Request Body:

json
Copy
{
  "email": "user@example.com",
  "password": "yourpassword"
}
Response:

json
Copy
{
  "token": "your-jwt-token"
}
🔧 Configuration
To configure this project, you will need the following tools:

MongoDB Atlas: For database hosting.
Node.js: The runtime for the backend.
React: For the frontend.
Axios: For making HTTP requests from the frontend.
🎨 Frontend Screenshots
1. Job Listings Page:

2. Job Detail Page:

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

💬 Contributing
Contributions are welcome! If you'd like to help improve JobHive, feel free to fork the repository and submit a pull request. Here’s how you can contribute:

Fork the repo.
Create a new branch.
Commit your changes.
Push to the branch.
Open a pull request.
👨‍💻 Authors
Patience Nkatha - my project - nkatha1
📜 Acknowledgements
MongoDB for providing a cloud-based database solution.
Node.js and Express.js for backend development.
React for making the frontend interactive.
Material-UI for easy-to-use components.
