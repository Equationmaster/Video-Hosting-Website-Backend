**Video Hosting Website Backend**

Welcome to the backend of our video hosting website, a comprehensive platform designed to emulate the functionalities of popular video-sharing services like YouTube. This backend is built using modern technologies and follows best practices to ensure scalability, security, and performance.

**Project Overview**

This project serves as the backend for a video hosting website, implementing core features such as user authentication, video upload, commenting, subscriptions, and more. The backend is built with Node.js and Express.js, utilizing MongoDB as the database to manage data efficiently. It incorporates industry-standard practices like JWT for secure authentication, bcrypt for password hashing, and proper use of access and refresh tokens for session management.

**Features**

- **User Authentication**: Sign up, login, logout, and password recovery using JWT and bcrypt.
- **Video Management**: Upload, edit, delete, and list videos.
- **Interactions**: Like, dislike, comment, reply to comments, and view video statistics.
- **Subscription System**: Subscribe and unsubscribe to channels, notifications for new videos.
- **Secure Authentication**: Use of access tokens and refresh tokens for managing user sessions.
- **Scalability**: Built to handle a large number of concurrent users and high traffic volume.

**Technologies Used**

- **Node.js**: Server-side JavaScript runtime environment.
- **Express.js**: Web framework for Node.js to build the RESTful API.
- **MongoDB**: NoSQL database for data storage.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js.
- **JWT (JSON Web Tokens)**: For secure user authentication.
- **Bcrypt**: For hashing passwords securely.
- **Multer**: For handling file uploads.
- **Cloudinary (or any cloud storage service)**: For storing and serving videos and images.

**Authentication and Security**

- **JWT Authentication**: Uses access tokens for secure, stateless user authentication. Refresh tokens are used to obtain new access tokens without requiring the user to log in again.
- **Password Hashing**: User passwords are securely hashed using bcrypt.
- **Role-based Access Control**: Different access levels for users and administrators to ensure proper authorization.\


**API Endpoints**

|**Method**|**Endpoint**|**Description**|
| :- | :- | :- |
|POST|/api/users/register|Register a new user|
|POST|/api/users/login|Login an existing user|
|POST|/api/users/logout|Logout the user|
|POST|/api/users/refresh-token|Refresh the access token|
|GET|/api/users/current-user|Get the current user|
|PATCH|/api/users/update-account  |Update account details|
|PATCH|/api/users/avatar|Update avatar|
|PATCH|/api/users/cover-image|Update cover image|
|POST|/api/users/changepassword |Change Current Password|
|GET|/api/users/history|Get Watch History|
|GET|/api/users/username|Get User channel name|

The Schema for the project is here:

https://app.eraser.io/workspace/FzjGkrRxs9q8kIx7y2pa?origin=share