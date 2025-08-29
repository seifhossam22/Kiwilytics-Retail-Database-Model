# Retail Database: Data Modeling Project
This project focuses on the design and documentation of a relational database schema for a retail business. The goal is to create a clean, organized, and scalable data model (ERD) that accurately represents the business's core entities and their relationships.

## Project Objective
The primary objective of this project was to design a robust data model that supports transactional operations and analytical queries for a retail business. The schema is built to manage key entities such as Orders, Products, Customers, and Employees, providing a solid foundation for data storage and retrieval.

## Schema Overview
The provided Entity-Relationship Diagram (ERD) illustrates the design, which includes the following tables:

- Orders: A central fact table that records each transaction. It links to Customers, Employees, and Shippers.

- Order_Details: A supporting table that breaks down each order into individual line items, linking to Orders and Products.

- Customers: Stores customer information.

- Employees: Stores employee details, including a self-referencing relationship for managers.

- Shippers: Contains details of shipping companies.

- Products: Stores information about the products sold, with a foreign key to the Categories table.

- Categories: Classifies products.

- Suppliers: Stores details of product suppliers.

## Key Relationships
The model is designed around clear relationships between these entities, ensuring data integrity and simplifying data retrieval:

### One-to-Many:

- One Customer can have many Orders.

- One Employee can be associated with many Orders.

- One Shipper can handle many Orders.

- One Category can contain many Products.

- One Supplier can provide many Products.

### Many-to-Many:

- The relationship between Orders and Products is handled by the Order_Details junction table.

## Technologies and Tools
- Data Modeling: Entity-Relationship Diagram (ERD)

- Database: Relational Database Management System (RDBMS)

## Project Deliverables
- ERD: The conceptual and logical design of the database schema.
