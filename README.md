ChatGPT Clone (MERN + Claude API)

A ChatGPT-like AI chatbot built with the MERN stack, using Claude APIs for AI responses.

Features

PWA with offline support
Authentication (Password, Google login)
Chat with auto-save & history
Account management (Forgot password, Delete account)
Dark/Light mode
Responsive design
Prerequisites

Node.js
AWS DocumentDB
Git
Claude API key from Anthropic
AWS EC2 instance for deployment
Tech Stack

Frontend: Vite, React.js, SCSS, Redux Toolkit
Backend: Node.js, Express.js, AWS DocumentDB, JWT authentication
AI: Claude API
Email: Gmail SMTP with Nodemailer
Environment Variables

Server (.env)

PORT=5000  
DOCDB_URL=your_documentdb_connection_string  
SITE_URL=your_site_url  
JWT_PRIVATE_KEY=your_jwt_key  
CLAUDE_API_KEY=your_claude_api_key  
MAIL_EMAIL=your_gmail_email  
MAIL_SECRET=your_gmail_app_password  
Client (.env.local)

VITE_CLIENT_ID=your_google_client_id  
Setup

Clone the project:

git clone https://github.com/your-repo.git  
Backend
cd ChatGPT/server  
npm install  
npm start  
Frontend
cd ChatGPT/client  
npm install  
npm run dev  
Deployment on AWS EC2

Set up an EC2 instance with Node.js and MongoDB-compatible AWS DocumentDB.
Configure security groups to allow necessary ports.
Deploy the backend and frontend on the EC2 instance.
Use a process manager like PM2 to keep the server running.
Authors

Adarsh Pallav & Ritesh Bhambhani
