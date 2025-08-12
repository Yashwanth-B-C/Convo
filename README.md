# Convo: A Real-time Group and Direct Chat Application

Convo is a full-stack, real-time chat application built with Node.js and Socket.io. It provides users with a platform for instant communication through both public group chats and private direct messages.

## Features

  * **User Authentication:** Secure signup and login for all users.
  * **Real-time Group Chat:** Join existing groups or create new ones to chat with multiple people simultaneously.
  * **Direct Messaging:** Send and receive private, one-on-one messages with other connected users.
  * **File Uploads:** The application supports file sharing, allowing users to upload and share files within chats.
  * **Persistent Storage:** All chat messages are stored in a database, ensuring that chat history is preserved.
  * **User Presence:** Tracks online users to enable and facilitate direct messaging.
  * **Scheduled Tasks:** Includes a cron job for automated maintenance, such as archiving old chats.

## Technologies Used

  * **Backend:**
      * **Node.js:** The server-side runtime environment.
      * **Express.js:** Web framework for handling API routes and server logic.
      * **Socket.io:** A library for real-time, bidirectional event-based communication.
      * **body-parser:** Middleware to parse incoming request bodies.
      * **dotenv:** To manage and load environment variables from a `.env` file.
  * **Database:**
      * **MySQL (or similar):** A relational database is used to store user data, messages, and group information.
  * **Frontend:**
      * **HTML, CSS, JavaScript:** Standard web technologies for the user interface.

## Getting Started

### Prerequisites

  * Node.js (LTS version recommended)
  * A MySQL database server

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repository.git
    cd your-repository
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Database Setup:**
      * Create a MySQL database for the project.
      * Update your database connection details in the `models/index.js` file or your `.env` file. You will need to create the necessary tables, such as `users`, `groups`, `messages`, and `direct_messages`.
4.  **Environment Variables:**
      * Create a `.env` file in the root directory of your project.
      * Add your port and database credentials to this file:
    <!-- end list -->
    ```env
    PORT=3000
    DB_HOST=localhost
    DB_USER=root
    DB_PASSWORD=your_password
    DB_DATABASE=your_database_name
    ```

### Running the Application

1.  **Start the server:**
    ```bash
    npm start
    ```
2.  **Access the application:**
      * Open your web browser and navigate to `http://localhost:3000`. You will be redirected to the signup page.

## Project Structure

  * `app.js`: The main server file that handles all routes, Socket.io connections, and server startup.
  * `public/`: Contains static client-side files like `signup.html`, `login.html`, `chat.html`, and their associated CSS/JS.
  * `routes/`: Houses the Express route handlers for authentication, chat, and file uploads.
  * `models/`: Contains the database connection configuration.
  * `cron/`: Contains scripts for scheduled tasks, such as `archiveChats.js`.

## Contributing

Contributions are welcome\! Please feel free to open an issue or submit a pull request.

## Screenshots

<img width="1054" height="826" alt="Screenshot 2025-08-06 194353" src="https://github.com/user-attachments/assets/49165cc1-f889-4241-8234-e6c5010633b1" />

<img width="1794" height="953" alt="Screenshot 2025-08-06 194436" src="https://github.com/user-attachments/assets/bd5a4a3c-54ca-4c5f-9cf1-256dbe029f51" />

<img width="1714" height="835" alt="Screenshot 2025-08-06 194455" src="https://github.com/user-attachments/assets/1b9dc018-f258-469e-9332-e630ea8affe2" />

<img width="1893" height="936" alt="Screenshot 2025-08-06 194702" src="https://github.com/user-attachments/assets/31a421c7-9e16-4b8f-9e19-56db14efa461" />

<img width="1889" height="816" alt="Screenshot 2025-08-06 194750" src="https://github.com/user-attachments/assets/910e8e46-4543-4822-b367-e34ad8e18b8d" />

<img width="1912" height="789" alt="Screenshot 2025-08-06 194808" src="https://github.com/user-attachments/assets/c6e06921-8e70-4120-89e2-fad4413f4935" />

<img width="1915" height="821" alt="Screenshot 2025-08-06 194903" src="https://github.com/user-attachments/assets/4545e77b-b9f9-4b87-8c95-d0780d0e63b8" />

<img width="1911" height="1015" alt="Screenshot 2025-08-06 194957" src="https://github.com/user-attachments/assets/0effea56-3b34-4bfb-a11f-7eb393be1cab" />

<img width="1842" height="857" alt="Screenshot 2025-08-06 195043" src="https://github.com/user-attachments/assets/fd746126-4877-4316-b90e-1aa51b74ea85" />

<img width="1905" height="901" alt="Screenshot 2025-08-06 195136" src="https://github.com/user-attachments/assets/a24a4bc9-3f01-4df7-9609-4d67a776119e" />

<img width="1913" height="935" alt="Screenshot 2025-08-06 195151" src="https://github.com/user-attachments/assets/465ff08f-f846-42f2-86c4-9136a0aac481" />

<img width="1917" height="1025" alt="Screenshot 2025-08-06 195354" src="https://github.com/user-attachments/assets/27d8ed2e-3695-42b2-b92a-b1c30b49f4f9" />
