## Portfolio Platform using Node.js

This project is a portfolio platform built using Node.js, Express, EJS, and MongoDB. It provides functionalities for user registration, login, authorization, API integration, and email sending using Nodemailer.

### Features

* **User Management:**
    * User registration with username, password, and optional information (First Name, Last Name, Age, Country, Gender).
    * Secure user login with password hashing using bcrypt.
    * User roles (admin and regular user) for authorization purposes.
* **Portfolio Management:**
    * Admin-only functionality to add, edit, and delete portfolio items.
    * Each item includes three images, two names (for different languages), two descriptions (for different languages), and timestamps for creation, update, and deletion.
    * On the main page, items are displayed in well-designed blocks with carousels for images and details.
* **API Integration:**
    * Three different pages utilize APIs to display visually appealing charts or graphs, providing insights and user engagement.
* **Email Notifications:**
    * Welcome email sent after successful user registration.
    * (Optional) Additional notifications for specific actions within the platform.

### Setup Instructions

1. **Prerequisites:**
    * Node.js and npm installed on your system.
    * MongoDB database instance running locally or remotely with appropriate IP access granted.
2. **Clone the repository:**

   ```bash
   git clone <repository_url>
   ```

3. **Install dependencies:**

   ```bash
   cd portfolio-platform
   npm install
   ```

4. **Environment variables:**

   Create a `.env` file in the project root directory and add the following environment variables with your specific details:

   ```
   DB_URI=<your_mongodb_connection_string>
   SECRET_KEY=<your_secret_key>
   ADMIN_USERNAME=<your_admin_username>
   ADMIN_PASSWORD=<your_admin_password>  **Note:** Do not store the actual password here. Use a secure method like environment variables and access them securely in your code.
   ```

5. **Start the application:**

   ```bash
   npm start
   ```

   This will start the server on port 3000 by default. You can access the application in your browser at `http://localhost:3000`.

### API Usage

The application uses the following APIs for data visualization:

* **API 1:** Unplash API
* **API 2:** randomuser API
* **API 3:** quotes-inspirational API

### Design Decisions

* EJS is used for templating to separate server-side logic from presentation.
* Responsive design is implemented for optimal viewing across different devices.
* User interface incorporates thoughtful design elements to enhance user experience.

### Deployment

For production deployment, consider using platforms like Heroku or AWS to host the application and configure environment variables securely.

### Contributing

**Note:** This project is intended for individual completion. 

### License

This project is licensed under the MIT License.

### Author

**Name:** Kassen Ilyas
**Group Number:** SE-2212

**Note:** Replace the bracketed information with your own details. Remember to remove the placeholder for the admin password and use a secure method to store it.
