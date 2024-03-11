# Social Media Dashboard

This project is a simple social media dashboard application with user registration, login, and the ability to create, view, edit, and delete posts. The application uses Node.js for the server-side logic, Express.js for routing, MongoDB for data storage, and JWT for authentication.

## Prerequisites
Ensure you have the following software installed on your machine
- Node.js
- npm
- Docker

## Getting Started
1. Clone the repository:
```
git clone https://github.com/AnuraagReddy123/Social-Media-Dashboard.git
```
2. Navigate the project directory
```
cd social-media-dashboard
```
3. Install dependencies
```
npm i
```
4. Run the application
```
node app.js
```

## Configuration
Make sure to set the following environment variables for the application to work correctly. You can either create a .env file or directly set these variables:
- `PORT`: Port number for the Node.js server (default: 3000)
- `SECRET_KEY`: Secret key for JWT token generation


## Usage
1. Visit http://localhost:3000/register to create a new user account.
2. After registration, log in at http://localhost:3000/login.
3. Once logged in, you can create, view, edit, and delete posts at http://localhost:3000/post.
4. Logout by visiting http://localhost:3000/logout.


## Endpoints
- POST /register: Create a new user account.
- POST /login: Log in with existing credentials.
- GET /post: View posts (authentication required).
- POST /post: Create a new post (authentication required).
- PUT /post/:postId: Update an existing post (authentication required).
- DELETE /post/:postId: Delete an existing post (authentication required).
- GET /logout: Log out the current user.

## Docker
This project includes a Dockerfile for containerization. Use the following commands to build and run the Docker container:
```
docker-compose build
docker-compose up
```
Visit http://localhost:3000 to access the application.

## Contribution
Feel free to contribute to the project. Fork the repository, make your changes, and submit a pull request.
