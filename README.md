## 🏗️ Project Description

This repository contains a full-stack application consisting of two main components: a React-based frontend and a backend API server. The frontend is built with React and provides the user interface for interacting with the application, while the backend is an API server that handles data storage and processing. These two components communicate with each other via HTTP requests and need to be run separately. The project uses MongoDB as the database for storing application data. To get started, you will need to set up both the frontend and backend, configure the necessary environment variables, and ensure that the correct versions of Node.js and MongoDB are installed.

## 🏗️ Project Structure

This repository consists of two applications:

- A React-based frontend
- A backend API server

These applications communicate via HTTP requests and must be run separately.

## 🚀 Quickstart

### 📥 Installing Node.js

If you haven't done so already, ensure that both Node.js and NVM are installed.

1. Install Node Version Manager (NVM)
   ```
   brew install nvm
   ```
   Follow the instructions to update your `~/.bash_profile`.

2. Open a new terminal session.
3. Install the latest version of [Node.js](https://nodejs.org/en/) (currently `24.0.2`):

   ```
   nvm install 24
   ```

### 🛠️ Project Setup

1. Fork this repository.
2. Clone the forked repository to your local machine.
3. Install the dependencies for both the `frontend` and `api` applications:
   ```
   cd frontend
   npm install
   cd ../api
   npm install
   ```
4. Install an ESLint plugin for your code editor, such as 
   [ESLint for VSCode](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint).
5. Install MongoDB

   ```
   brew tap mongodb/brew
   brew install mongodb-community@6.0
   ```

   _Important:_ If you see a message saying:
   `If you need to have mongodb-community@6.0 first in your PATH, run:`
   follow the instructions provided and restart your terminal after completing the steps.
6. Start MongoDB

   ```
   brew services start mongodb-community@6.0
   ```

### ⚙️ Configuring Environment Variables

You need to create two `.env` files — one for the frontend and one for the backend.

#### Frontend

Create a file `frontend/.env` with the following content:

```
VITE_BACKEND_URL="http://localhost:3000"
```

#### Backend

Create a file named `api/.env` with the following content:

```
MONGODB_URL="mongodb://0.0.0.0/acebook"
NODE_ENV="development"
JWT_SECRET="secret"
```

## 🏃‍♂️ Running the Application

1. Start the backend API server (located in the `api` directory) in development mode:

```
; cd api
; npm run dev
```

2. In a new terminal session, start the frontend application (located in the `frontend` directory):

In a new terminal session...

```
; cd frontend
; npm run dev
```

Now, open your browser and visit `http://localhost:5173/signup` to create a new user.

After signing up, you can log in by going to `http://localhost:5173/login`.

## 👥 Contributors

- [@jackmisner](https://github.com/jackmisner)
- [@amritpalc](https://github.com/AmritpalC)
- [@aysinakpinar](https://github.com/aysinakpinar)
- [@Michal-P-1](https://github.com/Michal-P-1)
- [@AMcGill3](https://github.com/AMcGill3)
- [@zameermohamed](https://github.com/zameermohamed)
- [@ziaxgit](https://github.com/ziaxgit)
