# Project Title: Online Bookstore Management System

Project Description:
You are tasked with building an Online Bookstore Management System, where users can browse, search, and purchase books. 

## Key Features:

### User Authentication:

Implement user registration and login functionality using JWT authentication.
Users should be able to register, login, and logout securely.

### Book Management:

Implement CRUD operations for managing books **(Create, Read, Update, Delete).**
Each book should have attributes like title, author, genre, price, etc.
Only *authenticated* users should be able to perform CRUD operations on books.

### Shopping Cart:

Allow users to add books to their shopping cart.
Users should be able to view their cart, update quantities, and remove items.

### Checkout Process:

Implement a checkout process where users can review their cart and proceed to purchase.
Upon successful purchase, update the database to reflect the changes in inventory.

> Note: Create a dummy purchase process, no need for any kind of real transactions. When users proceed to checkout, instead of processing real payments, you can display a confirmation message indicating that the purchase was successful.

### Search and Filter:

Implement search functionality to search for books by title, author, or genre.

### Dashboard:

Provide a dashboard where users can view book information, order history, and manage their account.

### Error Handling and Validation:

Implement appropriate error handling and validation for user inputs, form submissions, and database operations.
Middleware:

Use middlewares for authentication, error handling, logging, etc., to enhance security and maintainability.

### Database Integration:

Utilize Sequelize ORM to interact with the SQL database for storing user information, books, orders, etc.

### Views:

Render dynamic HTML views using EJS/Pug templates to display book listings, user profile, shopping cart, etc.
> You can use any view design that you want - no specifications here.

### Advanced Features to be supproted

You need to add the following after finalizing core feature implementation:
- _Unit Testing_: Implement unit tests for controllers, models, and middleware.
    - P0: Critical tests covering essential functionalities like authentication and CRUD operations.
    - P1: Additional tests for edge cases, error handling, and optional features.
    - P0 tests should run per commit and P1 should run for the PRs on the master branch before deployment.
- _Logging_: Integrate logging to track errors, user activities, and system behavior.
    - Logger needs to have a specific format *<timestamp><file><function>*
- _Dockerization:_ You need to dockerize the app by implementing needed files like **Dockerfile** and **docker_compose** ones. You then need to build and deploy the image.
- _Monitoring:_ Choose a monirotin tool of your choice (Grafana. Prometheus, etc) to track some API metrics like **(choose 2-3 metrics and implement them)**
    - Directly connect Grafana to your SQL database to run queries and visualize data.
    - Collect and store metrics from your application and infrastructure.
    - Track user activities such as logins, sign-ups, and purchases.
    - Visualize trends in user behavior over time.
    - Visualize metrics like query execution times, database load, and the number of active connections.
    - Monitor the performance of critical endpoints such as user authentication, product listing, and checkout.

### Additional Features (Bonus):

Implement pagination for book listings.
Add sorting options for book listings (e.g., sort by price, title, etc.).
Implement role-based access control for admin functionalities.

Project Structure:

* Separate your project into MVC components: models, views, and controllers.
* Utilize TypeScript for implementing the backend logic to leverage its type checking features.
* Organize your routes using `Express.js`.
* Use appropriate folder structures and naming conventions to maintain code cleanliness and readability.
