# E-commerce_follow_along

### Milestone 1 ###

•Features

⁕Authentication Page

-User Login and Signup functionality.
-Password security.
-Token-based authentication for session management.


⁕Product Page

-Displays a list of available products.
-Search and filter functionality for efficient product browsing.


⁕Order Page

-View all past orders with relevant details (product name, price, date).
-Track the status of current orders.


⁕Payment Gateway

-Multiple payment methods (credit/debit card, UPI, wallet).
-Secure transaction handling.
-Mock payment integration for testing.


⁕Tech Stack

1. Frontend
-React: For building an interactive and dynamic user interface.
-Next.js: For server-side rendering and improving performance.

2. Backend
-Express.js: For building the RESTful API to handle business logic.
-Mongoose: For managing the MongoDB database and creating schemas.

3. Database
-MongoDB: To store user information, product data, orders, and payment records.

### Milestone 2 ###
1. Created a structured folder hierarchy for the project.
2. Set up a React app for the frontend.
3. Set up a Node.js server for the backend.
4. Configured Tailwind CSS for streamlined styling.
5. Added optional extensions for improving development efficiency.
6. Built a functional and styled Login Page for the frontend.

### Milestone 3 ###

1. Set up dedicated folders for organizing backend code effectively.
2. Initialized and configured a Node.js server to handle API requests.
3. Connected the application to MongoDB to store and manage data.
4. Implemented basic error handling to ensure smooth server operation

## MILESTONE 4 ###
1. Create a User Model
Designed and implemented a User Model that serves as a blueprint for how user data is structured and stored in the database. This model defines the user schema and the fields that are needed for user-related data.
2. Create a User Controller
Developed a User Controller that handles the logic related to user data. It manages tasks such as adding a new user, retrieving user information, and other user-related operations.
3. Enable and Configure Multer for File Uploads
Configured Multer to handle file uploads in the application. This allows users to upload files (like images) which will be stored appropriately in the system. Multer is set up to handle storage configurations and file validation.

## MILESTONE 5 ###
1. Created a Sign-Up Page in React.
2. Implemented form validation for:
      Name (required)
      Email (valid format required)
      Password (minimum 2 characters)
      Password Confirmation (must match password)

4. Used React Router for navigation.

## Milestone 6: User Registration and Authentication
1. User Creation Endpoint (/create-user):
 Implemented an endpoint to create a new user.
 Validated the email to ensure the user doesn’t already exist.
 Successfully handled file uploads (e.g., avatar) using multer.

 2. Password Hashing:
 Used bcryptjs to hash passwords before saving them to the database, ensuring secure password storage.

4. Error Handling:
Incorporated centralized error handling using a custom ErrorHandler class.
Applied catchAsyncErrors middleware to manage asynchronous errors in the routes.

5. User Data Storage:
Stored user details (e.g., name, email, password, avatar) in MongoDB with encrypted password.

6. Email Notification (Optional):
Integrated an email notification system to send a welcome email to the user after successful registration (using sendMail).

7. JWT Token Generation:
Added a method to generate JWT tokens upon user login (for future use in authentication routes).

### Milestone 7: Create Login Endpoint
Task Completed ✅
Implemented a login API endpoint.
Accepted user credentials (email/username and password).
Retrieved the corresponding user from the database.
Validated the password using bcrypt.
Compared the entered password with the stored hashed password for authentication.
Generated a JWT token upon successful login for authentication.
Implemented error handling for invalid credentials and server errors.

### Milestone 8: Product Card Component

## Overview

In Milestone 8, we focus on creating a reusable product card component and designing a homepage to display a collection of these cards. Each card will showcase key product details, such as the product's name, price, and image. The goal is to create a clean and organized layout that improves the user experience and allows for easy browsing of products. This milestone demonstrates the principles of component-based design and how to efficiently manage dynamic content within your app.

## Features

Reusable Product Card: A single card component that accepts dynamic product details as props and renders them in a uniform, visually appealing way. The product card includes:

1. Product name
2. Product image
3. Product price

Dynamic Rendering: Use of JavaScript array mapping to iterate through a list of products and dynamically render each product's card with its respective data.
Homepage Layout: A structured layout, designed using either CSS Grid or Flexbox, to display multiple cards on the homepage in a responsive, organized manner.
Consistent Design: The card component ensures that the product details are presented consistently across all cards, providing a seamless user experience

### Milestone 9: Create Product Component

## Overview

In this milestone, we have implemented the Create Product component for the Follow-Along Ecommerce project. This component allows users to create new products by entering details such as name, description, category, tags, price, stock, email, and uploading images.

## Features Implemented

*Form Inputs:* Users can input product details including name, description, category, tags, price, stock, and email.

*Image Upload & Preview:* Users can upload multiple images, which will be displayed as previews before submission.

*Category Selection:* A dropdown to choose a product category.

*Validation & Submission:* Required fields are enforced, and product data is logged on submission.

*Memory Optimization:* Object URLs for image previews are revoked to prevent memory leaks.

## Technologies Used

*React:* Functional components and hooks (useState, useEffect).

*Tailwind CSS:* For styling.

*React Icons:* AiOutlinePlusCircle for the image upload button.