## Library Management System (SQL)

## Objective

- The goal of this project is to create a Library Management System database that will store information about books, authors, and members.
- This will involve creating the database, defining tables, and populating them with sample data.

## Tools Used

- SQL Server

## Database Structure
      
- ### Authors Table

- AuthorID(INT, Primary Key, Auto-increment)
- FirstName(NVARCHAR(50), NOT NULL)
- LastName(NVARCHAR(50), NOT NULL)
- BirthDate(DATE)
  
- ### Books Table

- BookID(INT, Primary Key, Auto-increment)
- Title(NVARCHAR(100), NOT NULL)
- AuthorID(INT, Foreign Key referencing Authors)
- PublicationYear (YEAR)
- Genre(NVARCHAR(50))
  
- ###  Members Table
  
- MemberID(INT, Primary Key, Auto-increment)
- FullName(NVARCHAR(100), NOT NULL)
- MembershipDate (DATE)
- Email(NVARCHAR(100))
  
- ### Transaction Table

- TransactionID (INT, Primary Key, Auto-increment)
- BookID (INT, Foreign Key referencing Books)
- MemberID (INT Foreign Key referencing Members)
- BorrowDate (DATE, NOT NULL)
- ReturnDate (DATE NULL)

## Features

- Add and manage books
- Track issued and returned books
- Query available books

## Sample Queries
      
- Retrieve Authors
- Retrieve Books
- Retrieve Members
- Check Transaction History

## Summary

- In this project, we successfully created a LibraryDB database, defined tables for authors, books, members, and inserted sample data.
- This foundational setup can be expanded with additional features such as:
- Transactions: Handling book loans.
- SearchFunctionality: Finding books or members.


## Author
      
- Aishika Nandy
