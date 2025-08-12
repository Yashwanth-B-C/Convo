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
    git https://github.com/Yashwanth-B-C/Convo.git
    cd Convo
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

<img width="1054" height="826" alt="Screenshot 2025-08-06 194353" src="https://github.com/user-attachments/assets/a47e67c6-98d5-4a53-9c07-19510c424cd3" />

<img width="1794" height="953" alt="Screenshot 2025-08-06 194436" src="https://github.com/user-attachments/assets/5264ffe8-b730-4a8a-96b9-59cd01541a1c" />

<img width="1714" height="835" alt="Screenshot 2025-08-06 194455" src="https://github.com/user-attachments/assets/0fd794b7-3450-417b-b7f3-866a93f82938" />

<img width="1893" height="936" alt="Screenshot 2025-08-06 194702" src="https://github.com/user-attachments/assets/d7dbcee6-52bd-49fc-8beb-b4571d0bea71" />

<img width="1889" height="816" alt="Screenshot 2025-08-06 194750" src="https://github.com/user-attachments/assets/bf8d6404-76cd-4350-8257-8f0908c0a260" />

<img width="1912" height="789" alt="Screenshot 2025-08-06 194808" src="https://github.com/user-attachments/assets/23cfae68-33e8-4bc1-938b-1d84a688ba98" />

<img width="1915" height="821" alt="Screenshot 2025-08-06 194903" src="https://github.com/user-attachments/assets/8f2c9a44-55dd-49be-b406-7c47a5e9a1bd" />

<img width="1911" height="1015" alt="Screenshot 2025-08-06 194957" src="https://github.com/user-attachments/assets/a64c7420-5422-4072-8f55-e8328ba41420" />

<img width="1842" height="857" alt="Screenshot 2025-08-06 195043" src="https://github.com/user-attachments/assets/b394983f-eb1e-43a8-9c5c-a04621802a8c" />

<img width="1905" height="901" alt="Screenshot 2025-08-06 195136" src="https://github.com/user-attachments/assets/7f7c27ce-84e2-437d-89da-135bfd15e217" />

<img width="1913" height="935" alt="Screenshot 2025-08-06 195151" src="https://github.com/user-attachments/assets/b52ffdf5-6e79-499d-a345-4e360611668b" />

<img width="1917" height="1025" alt="Screenshot 2025-08-06 195354" src="https://github.com/user-attachments/assets/f59b12df-bdd5-4c95-a0dc-b4d48d6a7d56" />

