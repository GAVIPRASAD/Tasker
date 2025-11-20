# Task Manager App (Tasker)

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)

A robust Task Manager application built using the **MVC (Model-View-Controller)** architecture. This project provides a RESTful API for task management operations and includes a frontend interface for user interaction.

## 📋 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
- [Usage](#-usage)
- [API Endpoints](#-api-endpoints)
- [Contributing](#-contributing)

## 🚀 Features

- **Create Tasks**: Add new tasks to your list.
- **Read Tasks**: View all tasks or specific task details.
- **Update Tasks**: Mark tasks as completed or edit task names.
- **Delete Tasks**: Remove tasks permanently.
- **Persistent Storage**: All data is stored securely in MongoDB.
- **Responsive UI**: Simple HTML/CSS frontend served via the public directory.

## 🛠 Tech Stack

* **Backend**: Node.js, Express.js
* **Database**: MongoDB, Mongoose (ODM)
* **Frontend**: HTML5, CSS3, Vanilla JavaScript
* **Tools**: Postman (for API testing), Dotenv (environment variables)

## 📂 Project Structure

```bash
Tasker/
├── controllers/    # Route logic and controller methods
├── db/             # Database connection configuration
├── models/         # Mongoose Schema definitions
├── routes/         # API route definitions
├── middleware/     # Error handling and async wrappers
├── errors/         # Custom error classes
├── public/         # Static assets (Frontend UI)
├── app.js          # Main entry point of the application
└── package.json    # Project dependencies and scripts
```

## 🏁 Getting Started

Follow these instructions to set up the project on your local machine.

### Prerequisites

Ensure you have the following installed:
* [Node.js](https://nodejs.org/) (v14+ recommended)
* [MongoDB](https://www.mongodb.com/try/download/community) (or a MongoDB Atlas account)

### Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/GAVIPRASAD/Tasker.git](https://github.com/GAVIPRASAD/Tasker.git)
    cd Tasker
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

### Environment Variables

Create a `.env` file in the root directory to configure your database connection.

1.  Create a file named `.env`.
2.  Add the following variable:

```env
MONGO_URI=mongodb+srv://<your_username>:<your_password>@<your_cluster>.mongodb.net/TASK-MANAGER?retryWrites=true&w=majority
PORT=5000
```

## 🏃‍♂️ Usage

Start the development server:

```bash
npm start
```
*Or if you have nodemon installed:*
```bash
npm run dev
```

Once the server is running, open your browser and navigate to:
`http://localhost:5000`

## 🔌 API Endpoints

If you are using Postman or cURL to test the backend directly:

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **GET** | `/api/v1/tasks` | Get all tasks |
| **POST** | `/api/v1/tasks` | Create a new task |
| **GET** | `/api/v1/tasks/:id` | Get a single task by ID |
| **PATCH** | `/api/v1/tasks/:id` | Update a task (name/status) |
| **DELETE** | `/api/v1/tasks/:id` | Delete a task |

## 🤝 Contributing

Contributions are always welcome!

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
