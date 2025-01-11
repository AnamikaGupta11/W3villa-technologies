# Installation Manual for Backend Project

## Prerequisites
Ensure you have the following installed:

1. **Node.js**: Download and install from [Node.js official website](https://nodejs.org/).
2. **npm**: Comes bundled with Node.js. Verify installation by running:
   ```bash
   node -v
   npm -v
   ```
3. **MongoDB**: Install and ensure it is running on your local machine or accessible remotely.

## Installation Steps

### 1. Clone the Repository
Clone the project repository to your local machine:
```bash
git clone <repository-url>
```
Navigate into the project directory:
```bash
cd backend
```

Alternatively, you can download the project as a ZIP file:

1. Click on the "Code" button on the repository's page.
2. Select "Download ZIP."
3. Extract the ZIP file to your desired location.

### 2. Install Dependencies
Install the required dependencies using npm:
```bash
npm install
```

### 3. Set Up Environment Variables
Create a `.env` file in the root directory and configure the following variables:

```env
PORT=5000
MONGO_URI=<your-mongodb-connection-string>
JWT_SECRET=<your-jwt-secret>
EMAIL_HOST=<your-email-host>
EMAIL_PORT=<your-email-port>
EMAIL_USER=<your-email-username>
EMAIL_PASS=<your-email-password>
```

Replace the placeholder values with your actual configuration details.

### 4. Start the Application

#### Development Mode:
Use `nodemon` for automatic restarts during development:
```bash
npm run dev
```

#### Production Mode:
Start the application using Node.js:
```bash
npm start
```

The backend server will start, and by default, it will run on `http://localhost:5000` unless specified otherwise in the `.env` file.

## Dependencies Overview
- **bcryptjs**: For hashing passwords.
- **cors**: Enables Cross-Origin Resource Sharing.
- **dotenv**: Loads environment variables.
- **express**: Web framework for building APIs.
- **jsonwebtoken**: For handling authentication tokens.
- **mongoose**: For MongoDB object modeling.
- **nodemailer**: For sending emails.

### Dev Dependencies
- **nodemon**: Automatically restarts the server during development.

## Troubleshooting

- **MongoDB Connection Errors:**
  - Ensure MongoDB is running.
  - Verify the `MONGO_URI` in the `.env` file.

- **Port Already in Use:**
  - If the default port (5000) is occupied, specify a different port in the `.env` file:
    ```env
    PORT=4000
    ```

- **Missing Environment Variables:**
  - Ensure the `.env` file is properly configured and saved.

For additional help, consult the project documentation or contact the maintainers.

