# Backend API

This project is a Backend API that provides various functionalities for a web application. It is built using Node.js and Express.js, and it interacts with a Microsoft SQL Server database. The API includes features such as user authentication using JSON Web Tokens (JWT), bcrypt for password hashing, and CORS support.
![GoogleGIF](https://github.com/Evanoken/simple_backend_encrypted_form/assets/95754975/e86302a7-955e-4a5e-a4ab-aa90ba1cb8f2)

## Installation

To install and run the Backend API on your local machine, please follow these steps:

1. Clone the repository from [GitHub](https://github.com/your-username/backend_API) to your local machine.

2. Navigate to the project directory.


3. Install the project dependencies using npm.


4. Set up the environment variables. Create a `.env` file in the root directory of the project and define the following variables:

DB_HOST=your_database_host
DB_USER=your_database_username
DB_PASSWORD=your_database_password
DB_DATABASE=your_database_name
JWT_SECRET=your_jwt_secret

5. Start the API server.


The server should now be running on `http://localhost:3000`.
![BolAliexpressGIF](https://github.com/Evanoken/simple_backend_encrypted_form/assets/95754975/513cbc60-d6ea-4276-b273-7dd099c79247)
## Usage

Once the server is running, you can interact with the Backend API by sending HTTP requests to the available endpoints. The API provides various routes for user authentication, data retrieval, creation, updating, and deletion.
![UseCodeBrendenPleaseCreeperMadeThisGIF](https://github.com/Evanoken/simple_backend_encrypted_form/assets/95754975/3a66db37-eb41-4150-bf82-df958cb410c0)

### Authentication

The following endpoints are available for user authentication:

- **POST /api/auth/register**: Register a new user by providing a username and password in the request body.
- **POST /api/auth/login**: Authenticate a user by providing a username and password in the request body. Returns a JWT token.
![DigibyteDgbGIF](https://github.com/Evanoken/simple_backend_encrypted_form/assets/95754975/ba230e4f-c52b-45c1-84d5-ce573ce15600)

### Protected Routes

The following endpoints require authentication using a JWT token:

- **GET /api/users**: Retrieve all users. Requires authentication as an admin user.
- **GET /api/users/:id**: Retrieve a specific user by ID. Requires authentication as an admin user.
- **PUT /api/users/:id**: Update a specific user by ID. Requires authentication as the user or an admin user.
- **DELETE /api/users/:id**: Delete a specific user by ID. Requires authentication as an admin user.

Please note that only admin users can access certain routes and perform specific operations.

You can use tools like cURL, Postman, or any HTTP client library to send requests to these endpoints.

## Scripts

The following scripts are available to manage the project:

- **start**: Starts the API server using `node index.js`.
- **dev**: Starts the API server with nodemon for development, automatically restarting the server when changes are made.

## Author

This project was developed by Evans Ngugi Kariuki.

![BrooklynNineNineAndySambergGIF](https://github.com/Evanoken/simple_backend_encrypted_form/assets/95754975/924328a6-d5ab-445c-8543-7ca8d5db217c)





