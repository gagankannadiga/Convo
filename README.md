# Convo: A Real-time Group and Direct Chat Application

Convo is a full-stack, real-time chat application built with **Node.js** and **Socket.io**. It provides users with a platform for instant communication through both public group chats and private direct messages.

-----

## Features

  * **User Authentication**: Secure signup and login for all users.
  * **Real-time Group Chat**: Join existing groups or create new ones to chat with multiple people simultaneously.
  * **Direct Messaging**: Send and receive private, one-on-one messages with other connected users.
  * **File Uploads**: The application supports file sharing, allowing users to upload and share files within chats.
  * **Persistent Storage**: All chat messages are stored in a database, ensuring that chat history is preserved.
  * **User Presence**: Tracks online users to enable and facilitate direct messaging.
  * **Scheduled Tasks**: Includes a cron job for automated maintenance, such as archiving old chats.

-----

## Technologies Used

### Backend

  * **Node.js**: The server-side runtime environment.
  * **Express.js**: Web framework for handling API routes and server logic.
  * **Socket.io**: A library for real-time, bidirectional event-based communication.
  * **body-parser**: Middleware to parse incoming request bodies.
  * **dotenv**: To manage and load environment variables from a `.env` file.

### Database

  * **MySQL (or similar)**: A relational database is used to store user data, messages, and group information.

### Frontend

  * **HTML, CSS, JavaScript**: Standard web technologies for the user interface.

-----

## Getting Started

### Prerequisites

  * Node.js (LTS version recommended)
  * A MySQL database server

### Installation

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/Yashwanth-B-C/Convo.git
    cd Convo
    ```
2.  **Install dependencies**:
    ```bash
    npm install
    ```
3.  **Database Setup**:
      * Create a MySQL database for the project.
      * Update your database connection details in the `models/index.js` file or your `.env` file. You will need to create the necessary tables, such as `users`, `groups`, `messages`, and `direct_messages`.
4.  **Environment Variables**:
      * Create a `.env` file in the root directory of your project.
      * Add your port and database credentials to this file:
    <!-- end list -->
    ```
    PORT=3000
    DB_HOST=localhost
    DB_USER=root
    DB_PASSWORD=your_password
    DB_DATABASE=your_database_name
    ```

-----

## Running the Application

1.  **Start the server**:
    ```bash
    npm start
    ```
2.  **Access the application**:
      * Open your web browser and navigate to `http://localhost:3000`. You will be redirected to the signup page.

-----

## Contributing

Contributions are welcome\! Please feel free to open an issue or submit a pull request.
