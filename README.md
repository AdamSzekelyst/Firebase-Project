# Flutter Task Management App

This project is a task management application that allows users to track and manage their tasks. The app is built using the **Flutter** framework and utilizes **Firebase** services for user authentication, database management, file storage, and real-time data updates.

## Technologies Used

- **Flutter**: For building the mobile application.
- **Firebase**:
  - **Firebase Authentication**: For user authentication and login.
  - **Firestore**: For storing and managing tasks.
  - **Firebase Storage**: For storing task-related images.
  - **Firebase Core**: For initializing Firebase in the Flutter app.

## Firebase Integration

Firebase plays a central role in this application, handling user authentication, task data storage, and file storage. Below, I explain how Firebase is used in the project:

### 1. Firebase Authentication

User registration and login are handled through **Firebase Authentication**. The application implements the following features:

- **Login**: Users can log in using their email and password.
- **Sign Up**: New users can create an account.
- **User ID**: Once authenticated, Firebase provides a unique user ID, which is used to associate tasks with the user.

### 2. Firestore

Firestore is used to store and manage tasks. Each task is stored as a document in a collection. The tasks are associated with the user ID to ensure that each user can only access their own tasks.

### 3. Firebase Storage

Firebase Storage is used to store task-related images. Each image is stored with a unique name and associated with the task ID.

### 4. Firebase Core

Firebase Core is used to initialize Firebase in the Flutter app. Initialization is done in the `main.dart` file.