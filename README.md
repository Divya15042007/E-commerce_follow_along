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


### Milestone 10: Product Management Enhancements


Milestone 10 focuses on refining the product creation and management process. This includes improving the form submission flow, handling errors effectively, and ensuring a seamless user experience.

Key Features Implemented

Form Submission & Error Handling

Implemented a structured form to capture product details including:

Name

Description

Price

Category

Tags

Stock

Email

Multiple Images

Integrated multiple image selection for better product representation.

Enhanced error handling using try-catch methods to catch and display errors during product creation.

Debugging tools added to log form data before submission for easier troubleshooting.

API Integration

Built a POST endpoint to receive and validate product data.

Used FormData to handle file uploads efficiently.

Sent form data to the backend API, ensuring proper request formatting (multipart/form-data).

Provided real-time feedback to users on successful product creation or errors encountered.

Why Validation & Error Handling?

Ensures only valid data is stored in the database.

Helps users identify and correct input mistakes quickly.

Prevents incomplete or invalid submissions, reducing inconsistencies in the system.

Technologies Used

React.js for frontend UI

Express.js for backend API handling

MongoDB & Mongoose for database storage

Axios for HTTP requests

Postman for API testing

Next Steps & Enhancements

Implement user authentication to restrict product uploads to authorized users.

Develop an admin panel to manage and moderate product listings.

Introduce real-time image preview and editing capabilities.

Optimize database indexing for faster search and retrieval.

Repository & Submission Details

GitHub Repository: [Your Repository Link Here]

Progress Summary: This milestone enhanced the product creation process by improving form submission, adding error handling, and integrating API communication.

Submission: The repository has been updated, and all changes have been pushed successfully.

## Milestone 11 - Dynamic Home Page with Product Data

### Overview
#### In this milestone, we will make the home page dynamic by fetching and displaying all products stored in MongoDB.

- We will write a backend API endpoint to retrieve product data.
- The frontend will call this API and display the products dynamically using the ProductCard component.
#### Learning Goals 🎯
By completing this milestone, you will learn:
- ✅ How to write an API endpoint to fetch data from MongoDB.
- ✅ How to receive and handle data on the frontend.
- ✅ How to display data dynamically using components.

### Steps to Complete Milestone 11 📝

1. Backend: Create an API Endpoint
- Create an API route in Express.js to fetch all products from MongoDB.
- Use Mongoose to retrieve the data.
- This API fetches all products and sends them in JSON format.
- The frontend will call this API to get the list of products.


2. Frontend: Fetch Product Data
- Create a function to fetch product data from the backend using fetch() or Axios.
- Store the data in a state variable.
- useEffect calls the API when the page loads.
- setProducts stores the fetched data.
- map() loops through the products and passes each to ProductCard.


3. Display Products Dynamically
- The ProductCard component will receive product data as a prop and display it.
- Displays product image, name, and price dynamically.

#### Final Outcome 🎉
- ✅ The backend API sends all product data.
- ✅ The frontend fetches this data.
- ✅ Products are dynamically displayed using the ProductCard component.

# Milestone 12: My Products Page

## Overview
In this milestone, we will create a "My Products" page that displays all products added by a user based on their email. We will accomplish this by writing a backend endpoint to fetch products from MongoDB filtered by the user's email and dynamically displaying them on the frontend using the previously created product card component.

## Learning Goals 🎯
By the end of this milestone, you will:

- Learn how to write an endpoint to filter and send data from MongoDB based on a user's email.
- Understand how to fetch and receive data on the frontend.
- Display data dynamically using a product card component.

## Steps to Complete Milestone 12 📝

### Backend:
1. *Create an endpoint* in your backend application that retrieves all products associated with a user's email from MongoDB.
2. *Filter products* based on the email provided in the request.
3. *Send the filtered data* as a response to the frontend.

### Frontend:
1. *Write a function* to fetch the filtered product data from the backend.
2. *Process the received data* and pass it to the product card component.
3. *Dynamically display* the products on the "My Products" page.

## Notes
- This lesson will help in understanding how to filter data based on specific constraints and send it to the client efficiently.
- Ensure proper error handling for scenarios where no products are found for a given email.

## Next Steps
- Enhance the UI with better styling and user experience.
- Implement pagination if needed for better performance.
- Add authentication checks to ensure only the logged-in user's products are displayed.

# Milestone 13 - Edit and Update Products in MongoDB

## 🌟 Overview
In this milestone, we have implemented the functionality to **edit** the uploaded products. Users can now modify existing product details and save the updates in the MongoDB database.

## 🎯 Learning Goals
By completing this milestone, we have learned:
- How to write an **endpoint** that updates existing data in MongoDB.
- How to **auto-fill a form** with previous data and allow users to edit it.
- How to handle update operations effectively in a **full-stack** application.

---

# Milestone 14 - Delete Products in MongoDB

## 🌟 Overview
In this milestone, we have implemented the functionality to **delete** products from MongoDB. Users can now remove existing products by clicking a delete button.

## 🎯 Learning Goals
By completing this milestone, we have learned:
- How to write an **endpoint** that deletes a product from MongoDB using a specific ID.
- How to handle delete operations effectively in a **full-stack** application.

---

### Milestone 15: Navbar Component Integration

In this milestone, we'll create and integrate a reusable Navbar component across all screens for smooth navigation.

#### Key Tasks:
- Create a Navbar with links to:
  - Home
  - My Products
  - Add Product
  - Cart
- Make the Navbar responsive.
- Add the Navbar to all pages for easy navigation.

This milestone teaches how to build and reuse a responsive Navbar for seamless navigation.

### Milestone 16: Product Info Page

In this milestone, we will create a page to display product details, choose quantity, and add to the cart.

#### Key Tasks:
- Create a page to display product data.
- Add a quantity selector.
- Implement an "Add to Cart" button.

This milestone focuses on building a functional product info page for users.

### Milestone 17: Add to Cart Backend  

In this milestone, we will create a backend endpoint to add products to the cart and store them in the database.  

#### Key Tasks:  
- Update the user schema to store cart products.  
- Create a cart schema to manage cart items.  
- Write an endpoint to receive and store product details in the cart.  

This milestone focuses on implementing backend cart functionality for seamless shopping.

### Milestone 18: Fetch Cart Items Backend  

In this milestone, we will create a backend endpoint to retrieve all products in a user's cart for display on the cart page.  

#### Key Tasks:  
- Create an endpoint to handle requests from the cart page.  
- Fetch all cart products using the user's email.  

This milestone focuses on implementing backend logic to retrieve cart items efficiently.

### Milestone 19: Cart Page UI and Quantity Control

In this milestone, we will create a cart page UI and add functionality to increase or decrease the quantity of products in the cart.

#### Key Tasks:
- Build a frontend cart page to display products fetched from the backend.
- Add options to increase and decrease product quantities with + and - buttons.
- Create backend endpoints to handle quantity adjustments.

This milestone enhances the cart functionality by allowing users to modify product quantities.

### Milestone 20: User Profile Page

In this milestone, we will build a frontend profile page to display user data and create a backend endpoint to retrieve that data.

#### Key Tasks:
- Create a backend endpoint to send user data using their email.
- Design a frontend profile page to display the user’s profile photo, name, email, and addresses.
- Add a section for addresses with an “Add Address” button, and display “No address found” if no address exists.

This milestone enhances the user experience by providing a profile page to view and manage their information.


### Milestone 21: Address Form Frontend Page 
# Overview
Create a frontend form to collect and store address details, including country, city, address1, address2, zip code, and address type.
# Steps 
Build the address form page.
Store input values in state.
Navigate to this form when clicking "Add Address" in the profile.




### Milestone 22 - Save Address in User Profile
# Overview
In this milestone, we created a backend endpoint to store user addresses in the database. The endpoint receives address details from the frontend form and appends them to the address array in the user collection.

# Learning Outcomes
1. Implemented an API endpoint to handle address storage.
2. Updated the user collection to include multiple addresses.
3. Strengthened backend skills for handling user profiles.
# Submission Details
1. Code pushed to GitHub repository.
2. Repository is publicly accessible.
3. This README summarizes the progress.
4. This milestone enhances the user experience by providing a profile page to view and manage their information.




# 🎯 Milestone 23: Place Order & Address Selection

## Overview

In this milestone, we have enhanced the checkout process by introducing a "Place Order" button in the cart. This feature allows users to proceed with their purchase by selecting a preferred delivery address, ensuring a seamless and convenient shopping experience.

## Features Implemented

"Place Order" Button: A dedicated button in the cart that initiates the order placement process.

Address Selection: Users can choose from their saved addresses or enter a new one before confirming their order.

Enhanced User Experience: A streamlined checkout flow for better navigation and convenience.

Order Confirmation: Once the address is selected, users receive an order confirmation message.

## Benefits

Simplified Checkout: Reduces the number of steps required to complete a purchase.

User-Friendly Interface: Ensures a smooth and intuitive process for selecting the delivery address.

Improved Order Accuracy: Helps in preventing errors by allowing users to review their address before confirming the order.


# Milestone 24 🚀  

## Overview  
In this milestone, we will create an Order Confirmation page to display order details.  

## Steps  
1. Show all products being ordered.  
2. Display the selected delivery address.  
3. Show the total cart value.  
4. Add a "Place Order" button at the bottom.  

### Note  
This milestone helps in understanding how to implement the place order functionality.


# Milestone 25 - Order Placement API 📝

## Steps to Implement

1. *Create an Endpoint:*
   - Develop an endpoint that accepts product details, user information, and address details.

2. *Retrieve User ID:*
   - Extract the user's email from the request data.
   - Use this email to fetch the corresponding _id from the MongoDB users collection.

3. *Store Order Details:*
   - For each product, create a unique order entry with the same address.
   - Use the existing Order schema to store these details in the MongoDB orders collection.

### Key Notes
✅ Efficient endpoint design for placing orders.  
✅ Ensures proper data structure and storage.  
✅ Enhances understanding of MongoDB data handling and endpoint creation.  

---

# Milestone 26 📝

### Steps to Fetch User Orders
1. Create an endpoint to receive the *user's email*.
2. Retrieve the *user's _id* using the provided email.
3. Fetch all orders linked to that *_id*.
4. Respond with the user's order details.

This endpoint will help you retrieve all orders for a specific user.



## README - Milestone 27: My Orders Page  

### Overview  
In this milestone, we created a *My Orders* page for our frontend. This page fetches and displays all user orders by sending a GET request to the my-orders endpoint using the user’s email.  

### Learning Goals 🎯  
- Implement a frontend page to display user orders.  
- Send a request to retrieve order data from the backend.  
- Integrate the *My Orders* page into the navbar for easy access.  

### Implementation Steps 📝  
1. Created a *My Orders* page.  
2. Sent a GET request to fetch user orders using their email.  
3. Displayed the retrieved orders on the page.  
4. Updated the navbar to include the *My Orders* page for better navigation.  

### Submission Guidelines 📥  
- Code pushed to the GitHub repository.  
- Repository is publicly accessible.  
- README updated with milestone details.  
- Repository link submitted as per guidelines.  

🚀 *Milestone 27 completed successfully!*



## README - Milestone 28: Cancel Order Feature  

### Overview  
In this milestone, we enhanced the *My Orders* page by adding a *Cancel Order* button and implemented a backend endpoint to handle order cancellations.  

### Learning Goals 🎯  
- Enable users to cancel placed orders.  
- Implement order cancellation logic in the frontend and backend.  
- Prevent the cancel button from appearing for already canceled orders.  

### Implementation Steps 📝  
1. Added a *Cancel Order* button for each order in the *My Orders* page.  
2. Ensured the button is hidden for already canceled orders.  
3. Created a backend endpoint to receive an order-id, find the order, update its status to *canceled*, and save the changes.  

### Submission Guidelines 📥  
- Code pushed to the GitHub repository.  
- Repository is publicly accessible.  
- README updated with milestone details.  
- Repository link submitted as per guidelines.  

🚀 *Milestone 28 completed successfully!*


## Milestone-29 ##

PayPal Integration - Setup Guide

Step 1: Create a PayPal Sandbox Account

Visit PayPal Developer Dashboard and sign in.

Go to Sandbox Accounts and create an account.
Copy and save the User ID.

Step 2: Get PayPal Client ID

Find your sandbox account and click Manage Accounts.
Copy and save the Client ID.

Step 3: Add Payment Options

On the Order Confirmation Page, add radio buttons for:
Cash on Delivery (COD)

Online Payment (PayPal)
Show PayPal buttons only when Online Payment is selected.



## Milestone-30 ##
PayPal Integration - Setup Guide

Step 1: Create a PayPal Sandbox Account

Visit PayPal Developer Dashboard and sign in.

Go to Sandbox Accounts and create an account.

Copy and save the User ID.

Step 2: Get PayPal Client ID

Find your sandbox account and click Manage Accounts.

Copy and save the Client ID.

Step 3: Add Payment Options

On the Order Confirmation Page, add radio buttons for:

Cash on Delivery (COD)

Online Payment (PayPal)

Show PayPal buttons only when Online Payment is selected.

Milestone 30: Implement PayPal Payment




Milestone 31: Global State with Redux
Set up Redux to manage the user's email globally.

Key Tasks:
Install react-redux.
Create store.js and userActions.js.
Configure userReducer to store email.
Wrap App with Provider.
This milestone enables centralized state management




### Milestone 32: Managing Global State in Login and Other Pages

# Overview

In this milestone, we will implement global state management for storing the email entered on the login page. The email will be stored using Redux and will be accessible across all pages using useSelector.





### Milestone 33 - JWT Token & Cookie Storage

# 1Overview

In this milestone, we will learn how to implement JWT (JSON Web Token) authentication in a Node.js application.
JWT is used to securely transmit information between parties as a JSON object.
We will generate a JWT token, store it inside an HTTP-only cookie, and send it to the client upon successful authentication.

# Learning Goals
By the end of this milestone, you will:
1. Learn how to create a JWT token.
2. Understand how to store tokens inside cookies for authentication.

### Features
1. Generate JWT Token using the jsonwebtoken package.
2. Store JWT Token in HTTP-only Cookies for better security.
3. Set Token Expiry using the maxAge property.
4. Send Token in Response to maintain user authentication