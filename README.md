# Software Engineering Project

## Project Overview

This project is a web-based application developed as part of the Software Engineering Project. The project is designed to simulate an e-commerce system for managing users, groups, products, sales, and other administrative tasks.

### Features

- User authentication with three types of accounts: admin, special user, and regular employee.
- Sales report generation and tracking.
- Product management, including adding, editing, and deleting products.
- Category management, including adding, editing, and deleting categories.
- User and group management, including adding, editing, and deleting users and groups.
- Profile and media management.
- Daily and monthly sales reporting.
- Account and password management for secure access.
- Configurable and dynamic components using AJAX.

## Project Structure

Below is a summary of key files in the project:

### Authentication and User Management

1. `auth.php` / `auth_v2.php`
   - Handles user authentication and session management to ensure secure access to the system.

2. `login_v2.php`
   - Processes user login and redirects users to their respective dashboards based on roles.

3. `logout.php`
   - Terminates user sessions and logs users out of the system.

4. `change_password.php`
   - Allows users to update their passwords securely.

5. `users.php`
   - Manages user data, including creating, editing, and deleting users.

6. `edit_user.php`
   - Enables admin or special users to modify existing user details.

7. `delete_user.php`
   - Allows admin to remove users from the system.

8. `add_user.php`
   - Provides the ability to add new users to the system.

### Product and Category Management

9. `product.php`
   - Manages the product catalog, allowing users to view, add, and update product listings.

10. `edit_product.php`
   - Provides functionality for editing product information, such as descriptions, prices, and stock.

11. `delete_product.php`
   - Allows admin to delete products from the catalog.

12. `add_product.php`
   - Enables the addition of new products to the catalog.

13. `categorie.php`
   - Manages product categories, allowing the addition, viewing, and organizing of product categories.

14. `edit_categorie.php`
   - Enables admin users to modify existing categories.

15. `delete_categorie.php`
   - Allows admin users to delete product categories.

### Group Management

16. `group.php`
   - Manages user groups, providing functionality to assign users to different groups based on roles or permissions.

17. `edit_group.php`
   - Allows admins to edit group information, such as group name or permissions.

18. `delete_group.php`
   - Provides functionality to delete user groups from the system.

19. `add_group.php`
   - Allows admins to create new user groups and assign users to those groups.

### Sales and Reports

20. `sales.php`
   - Handles sales transactions, allowing users to complete orders and track ongoing sales.

21. `daily_sales.php`
   - Generates daily sales reports, displaying a summary of transactions for the day.

22. `monthly_sales.php`
   - Generates monthly sales reports, displaying accumulated sales data for each month.

23. `sales_report.php`
   - Provides detailed reporting on sales, including product, quantity, price, and total amounts.

24. `sale_report_process.php`
   - Processes data involved in generating sales reports.

25. `edit_sale.php`
   - Allows admin or special users to modify existing sales transactions.

26. `delete_sale.php`
   - Enables admin users to remove sales records from the system.

27. `add_sale.php`
   - Allows admins and authorized users to add new sales transactions.

### Media Management

28. `media.php`
   - Handles media-related features, such as uploading and managing files related to products or user profiles.

29. `delete_media.php`
   - Allows admin to delete media files from the system.

30. `upload.php`
   - Handles file upload functionalities for media or other resources.

### Configuration and Utility Files

31. `config.php`
   - Contains configuration settings for the project, including database credentials and system-wide settings.

32. `database.php`
   - Manages database connection and querying, facilitating communication between the application and the database.

33. `functions.php`
   - A collection of utility functions used throughout the project to streamline common operations like formatting, data validation, and more.

34. `load.php`
   - A file responsible for loading necessary scripts, assets, or dynamic content into the application.

35. `session.php`
   - Manages user sessions, ensuring users are properly logged in and out, with session data securely maintained.

36. `sql.php`
   - Likely contains raw SQL queries used to interact with the database for various operations.

### General Dashboard and Admin

37. `home.php`
   - The main dashboard that provides an overview of the system, including sales summaries and navigation links for managing products, users, and categories.

38. `admin.php`
   - The central administration panel where admins can manage all aspects of the system, including user accounts, products, categories, and sales reports.

39. `index.php`
   - The entry point of the web application, handling user authentication and redirecting to the appropriate dashboards.

40. `ajax.php`
   - Handles various asynchronous requests in the system for faster page updates without full page reloads, such as loading data dynamically.

### Deletion Functions

Several files handle the deletion of various entities within the system:
   - `delete_categorie.php`: Deletes categories.
   - `delete_group.php`: Deletes groups.
   - `delete_media.php`: Deletes media files.
   - `delete_product.php`: Deletes products.
   - `delete_sale.php`: Deletes sales.
   - `delete_user.php`: Deletes users.

## Database Configuration

The project uses a MySQL database named `db`. Ensure the following login credentials for database access are correctly configured:

- **Admin Login Details**  
  - Username: `admin`  
  - Password: `admin`

- **Special User Login Details**  
  - Username: `special`  
  - Password: `special`

- **User (Employee) Login Details**  
  - Username: `user`  
  - Password: `user`

## Requirements

- **PHP Version**: 5.6.3 (or higher recommended)
- **MySQL Database**: Ensure you have the `db` database configured in your environment.

## Installation

1. Clone this repository to your web server.
2. Import the database dump into your MySQL database using the provided `db` name.
3. Adjust database connection settings in the `config.php` file.
4. Ensure your server meets the required PHP version.
5. Login using the provided credentials to access the system.

## Usage

1. **Login**:  
   Use one of the provided accounts to log in based on your role (admin, special user, or employee).

2. **Admin Panel**:  
   Admin users have full control over the system, including managing products, categories, groups, generating reports, and overseeing users.

3. **Special User Panel**:  
   Special users have limited administrative access, typically viewing reports and managing specific areas such as sales or products.

4. **Employee Panel**:  
   Employees can track sales, manage personal profiles, and view their activities within the system.

## Support

For any issues or questions regarding the project, please contact the project contributor.

## License

This project is licensed for educational purposes only as part of the Software Engineering Project.
