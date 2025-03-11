# e-commerce-follow-along
### *Project Overview: E-Commerce Application (MERN Stack)*
This project will guide you through building a full-stack e-commerce web application using the *MERN stack* (MongoDB, Express.js, React.js, Node.js). You will learn how to implement key functionalities such as *user authentication, **product management, and **order handling* while gaining hands-on experience with REST APIs, database schema design, and frontend development with React.

---

### *Key Features:*
- *User Authentication:* Secure login and registration with JWT.
- *Product Management:* CRUD operations for products, with features like filtering and sorting.
- *Order Handling:* Users can place and view orders.
- *REST API:* Build scalable API endpoints for managing users, products, and orders.
- *Frontend:* Responsive UI built with React for a smooth user experience.

---

### *Core Concepts:*
- *MERN Stack*: Using MongoDB, Express.js, React.js, and Node.js for full-stack development.
- *REST APIs*: Design and develop API endpoints for user and product management.
- *Authentication*: Implement secure login and session management.
- *Database Schema*: Design MongoDB schemas for users, products, and orders.

---

### *Next Steps:* 
1. Set up the *development environment* and install dependencies.
2. Implement a *basic server* using Node.js and Express.
3. Start building the *React frontend* and connect it to the backend.
4. Design *MongoDB schemas* for structured data storage.

This project will help you master the full-stack development process, from database to frontend, with a focus on scalability and user interaction.

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
4. Implemented basic error handling to ensure smooth server operation.

### Milestone 4 ###

This milestone focuses on implementing user data handling and file upload functionality. 

Key achievements include:  
1. User Model: Defined a blueprint for storing user data in the database, ensuring a consistent structure for user-related information.  
2. User Controller: Developed logic to manage user operations such as adding new users and retrieving user information.  
3. File Upload Setup: Integrated and configured Multer to enable file uploads (e.g., user profile images) and store them efficiently in the application.  

By completing this milestone, the application now supports user management and file uploads, enhancing its core functionality.

## MILESTONE 5 :-
1. Created a Sign-Up Page in React.
2. Implemented form validation for:
    Name (required)
    Email (valid format required)
    Password (minimum 2 characters)
    Password Confirmation (must match password)

4. Used React Router for navigation.

## Milestone 6 :-
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
Implemented error handling for invalid credentials and server errors.


## Milestone -8 Progress:
Three files were made:
1) Product.jsx in Components/auth to store info. about product details.
2) user.js
3) data/js
We have createrd a reusable card component with props for product details.

## Milestone 9: Create Product Component

Overview

In this milestone, we have implemented the Create Product component for the Follow-Along Ecommerce project. This component allows users to create new products by entering details such as name, description, category, tags, price, stock, email, and uploading images.

Features Implemented

Form Inputs: Users can input product details including name, description, category, tags, price, stock, and email.

Image Upload & Preview: Users can upload multiple images, which will be displayed as previews before submission.

Category Selection: A dropdown to choose a product category.

Validation & Submission: Required fields are enforced, and product data is logged on submission.

Memory Optimization: Object URLs for image previews are revoked to prevent memory leaks.

Technologies Used

React: Functional components and hooks (useState, useEffect).

Tailwind CSS: For styling.

React Icons: AiOutlinePlusCircle for the image upload button.

## ###Milestone 10: Product Management Enhancements


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

---

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
1. **Create an endpoint** in your backend application that retrieves all products associated with a user's email from MongoDB.
2. **Filter products** based on the email provided in the request.
3. **Send the filtered data** as a response to the frontend.

### Frontend:
1. **Write a function** to fetch the filtered product data from the backend.
2. **Process the received data** and pass it to the product card component.
3. **Dynamically display** the products on the "My Products" page.

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
In this milestone, we have implemented the functionality to **delete

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

### Milestone 19: 
## Cart Page

The cart page allows users to view their selected products and modify quantities using `+` and `-` buttons. Each product's name, price, and quantity are displayed. The quantity updates in real-time as users interact with the buttons. The backend provides a `PUT /cart/update` endpoint that handles quantity adjustments. It accepts a request body with `productId` and `newQuantity`, and responds with the updated cart. This feature ensures users can easily manage their cart before checkout. The cart page is fully integrated with the backend for smooth functionality and up-to-date data display.

### Miestone 20:
 ## Profile Page

The profile page allows users to view and manage their personal information. The backend provides a `GET /profile` endpoint to fetch user data, including profile photo, name, email, and address. The frontend displays the profile information in two sections: one for personal details (photo, name, email) and another for the address. If an address is available, it is shown; otherwise, the message "No address found" appears. An "Add Address" button is included for users to add their address. This feature helps users view and edit their profile in a simple, user-friendly interface.

### Milestone 21 - Address Form Implementation
### 🌟 Overview
Implemented an Address Form page to collect and store user address details.

### 🎯 Learning Goals
Create a frontend form to take user address details.
Capture country, city, address1, address2, zip code, and address type.
### Steps 📝
Created an address form page.
Managed input data using state.
Navigated to the form when clicking "Add Address" in the profile.
This milestone helps in understanding how to build and manage an address form.



### Milestone 22 - Backend Endpoint for Storing User Address
👋 Hey Kalvians! 🌟

In this milestone, we created a backend endpoint to store user addresses in their profile.

🎯 Learning Goals
Build an API endpoint for address storage.
Receive and process address data from the frontend.
Update the user collection by adding the address.
📝 Steps Implemented
✅ Created API Endpoint – Handled address submission.
✅ Processed Data – Extracted address details.
✅ Updated Database – Stored address in the user profile.
✅ Tested Endpoint – Verified with Postman/Bruno.

This milestone enhances backend API development skills. 🚀

### Milestone 23 - Place Order & Select Address Page

### 🌟 Overview

In this milestone, we will implement the “Place Order” feature, allowing users to select a delivery address and finalize their order.

### 🎯 Learning Goals
	•	Add a “Place Order” button to the cart.
	•	Create a “Select Address” page to choose a delivery address.
	•	Write a Mongoose schema to store order details.

### Steps 📝
	1.	Place Order Button:
	•	Add a “Place Order” button to the cart page.
	•	Navigate to the “Select Address” page on click.
	2.	Create Select Address Page:
	•	Display all user addresses on this page.
	•	Allow users to select one as the delivery address.
	3.	Backend Endpoint:
	•	Write an endpoint to fetch all user addresses.
	4.	Mongoose Schema:
	•	Define a schema to store order details, including the selected address and product items.

## Next Steps (Milestone 24 - Order Confirmation Page)

Display all ordered products.

Show the selected delivery address.

Display the total cart value.

Include a "Confirm Order" button at the bottom.

This milestone will help you understand how to implement the "Place Order" functionality effectively.

# Milestone 25 - Order Placement API 📝

## Steps to Implement

1. **Create an Endpoint:**
   - Develop an endpoint that accepts product details, user information, and address details.

2. **Retrieve User ID:**
   - Extract the user's email from the request data.
   - Use this email to fetch the corresponding `_id` from the MongoDB `users` collection.

3. **Store Order Details:**
   - For each product, create a unique order entry with the same address.
   - Use the existing `Order` schema to store these details in the MongoDB `orders` collection.

### Key Notes
✅ Efficient endpoint design for placing orders.  
✅ Ensures proper data structure and storage.  
✅ Enhances understanding of MongoDB data handling and endpoint creation.  

---