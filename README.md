# How to Start the System on Another Laptop

1. **Copy the Project Folder**  
   Download `Class Teacher Mangement System` folder to your new laptop.

2. **Install Node.js**  
   Download and install Node.js from [https://nodejs.org/](https://nodejs.org/) if not already installed.
   

4. **Open the Project in VSCode**  
   Open Visual Studio Code and open the project folder.

5. **Install Dependencies**  
   Open the terminal in VSCode and run:
   ```
   npm install
   ```

6. **Start the Backend Server**  
   In the terminal, run:
   ```
   npm start
   ```
   or for development with auto-reload:
   ```
   npm run dev
   ```

7. **Access the System**  
   Open your browser and go to:
   ```
   http://localhost:3000
   ```

8. **(Optional) Setup Database**  
   - Make sure MongoDB is installed and running.
   - Update the database connection string in your code if needed.

---

## Database Setup

Follow these steps to set up the MongoDB database for the system:

1. **Install MongoDB**  
   Download and install MongoDB Community Edition from [https://www.mongodb.com/try/download/community](https://www.mongodb.com/try/download/community).

2. **Start MongoDB Service**  
   - On Windows, open Command Prompt and run:
     ```
     net start MongoDB
     ```
   - Or, use MongoDB Compass or your preferred method to start the MongoDB server.

3. **Create Database (Optional)**  
   - By default, the system will create the database automatically when you run the server.
   - If you want to create it manually, open the MongoDB shell and run:
     ```
     use class_teacher_management
     ```

4. **Update Connection String**  
   - Open your project's configuration file (index.js`).
   - Update the `MONGODB_URI` or similar variable to match your MongoDB setup
     ```
     MONGODB_URI=mongodb://localhost:27017/class_teacher_management
     ```

5. **Verify Connection**  
   - Start your backend server.
   - Check the terminal for a successful database connection message.

   Admin Deafault Account:

   admin

   admin123
