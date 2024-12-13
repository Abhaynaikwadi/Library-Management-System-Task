
# Library Management System

This project is a Python-based Library Management System that allows administrators and users to manage books and borrowing requests. The system uses SQLite as the database and provides basic functionalities like adding users, listing books, and handling borrowing requests.

## Features

### Admin Functions:
- Create new library users.
- View all book borrowing requests.
- Approve or deny book borrowing requests.

### User Functions:
- View available books.
- Request to borrow a book for specific dates.
- View borrowing history.

## Requirements

- Python 3.8 or higher
- SQLite (comes pre-installed with Python)

## Installation

1. Clone the repository or download the `library_management.py` file.
2. Ensure Python 3 is installed on your machine. You can download it from [python.org](https://www.python.org/).

## Setup and Usage

### 1. Initialize the Database
The database will automatically be created when you run the program for the first time.

### 2. Run the Program
Run the following command in your terminal or command prompt:
```bash
python library_management.py
```

### 3. Use the Menu
Follow the interactive menu to perform actions as an admin or user.

### Admin Options:
- **Create User**: Add a new library user by providing their email and password.
- **View All Requests**: View all book borrowing requests.
- **Approve/Deny Request**: Approve or deny a borrowing request.

### User Options:
- **List Books**: View all available books in the library.
- **Request Book**: Request a book for specific dates (if available).
- **View Borrow History**: View your borrowing history.

### 4. Exit the Program
Choose `0` from the menu to exit the program.

## Database Schema

The following tables are used:
- **Users**: Stores user information (email, password).
- **Books**: Stores book information (title, author, availability).
- **Borrow Requests**: Tracks borrowing requests and their statuses.

## Notes

- Borrow requests are checked for overlapping dates to ensure a book cannot be borrowed by multiple users at the same time.
- Only available books can be borrowed.
- Requests are stored with a status of `Pending`, `Approved`, or `Denied`.

## Future Enhancements

- **JWT Authentication**: Implement JWT-based authentication for API endpoints.
- **Swagger Documentation**: Create detailed API documentation using tools like Swagger or Postman.
- **Export Borrow History**: Allow users to download their borrow history as a CSV file.

## Contributing

Feel free to fork the project and submit pull requests for improvements or new features.


---

Enjoy using the Library Management System!
