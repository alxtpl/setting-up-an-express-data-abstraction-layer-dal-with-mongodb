
# Tiered Bad Bank Application

## Description / Motivation
The Tiered Bad Bank Application is a full-stack banking app that allows users to perform basic banking operations, including creating accounts, managing balances, and viewing all registered accounts. This project is designed to help developers practice and understand the development of a secure banking interface, integrating Express.js, MongoDB, and Docker for seamless back-end and front-end connections. It addresses the need for a straightforward demo of CRUD operations and user data handling.

## Installation Guidelines
To get started with the application, follow these steps:
1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   ```
2. **Navigate to the project directory:**
   ```bash
   cd <project_folder>
   ```
3. **Install dependencies:**
   ```bash
   npm install
   ```
4. **Run MongoDB in Docker:**
   ```bash
   docker run -p 27017:27017 --name badbank -d mongo
   ```
5. **Start the application:**
   ```bash
   node index.js
   ```
6. **Testing Routes:**
   - **Create a new user account:**
     ```
     http://localhost:3000/account/create/alex/alex@example.com/password123
     ```
   - **View all users:**
     ```
     http://localhost:3000/account/all
     ```

## Screenshots
Below are some screenshots of the application in action:
- ![Screenshot of Create Account](https://raw.githubusercontent.com/alxtpl/setting-up-an-express-data-abstraction-layer-dal-with-mongodb/refs/heads/main/create.png)
- ![Screenshot of All Accounts](https://raw.githubusercontent.com/alxtpl/setting-up-an-express-data-abstraction-layer-dal-with-mongodb/refs/heads/main/all.png)

## Technology Used
The following technologies and tools were used to build this project:
- **Express.js** - for creating RESTful API routes and handling server functionality.
- **MongoDB** - for managing and storing user account data.
- **Docker** - for containerizing the MongoDB instance and ensuring easy database setup.
- **JavaScript** - for both client-side and server-side scripting.

## Features
- **Create Account** - Users can create accounts with unique emails.
- **View All Accounts** - Lists all users and their account details.
- **Update Balance** - Allows users to deposit and withdraw funds from their accounts.
- **Delete Account** - Users can delete their accounts.
- **Planned Features** - Additional features like account authentication are planned for future development.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
