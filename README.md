### Title
**An Online Shopping DB System: Unified Database Design, Operations Execution, and Streamlined Financial Reporting for Enhanced E-Commerce Experience**

### Overview
This SQL script creates and populates a database for an online shopping system. The script covers the complete process of initializing the database, defining tables, setting up sequences, and inserting sample data for various entities involved in an e-commerce environment, such as customers, products, orders, credit cards, invoices, reviews, and recommendations.

### Detailed Sections

#### 1. Database Initialization
The script begins by enabling server output for execution feedback. It then drops existing tables and sequences if they exist to ensure a clean slate for the new database structure.

#### 2. Sequence Creation
Sequences are created for auto-generating unique identifiers for each primary key in the tables:
- **customers_seq:** Starts at 20231
- **categories_seq:** Starts at 1
- **products_seq:** Starts at 100
- **orders_seq:** Starts at 1
- **creditcards_seq:** Starts at 5123456778
- **invoices_seq:** Starts at 1
- **reviews_seq:** Starts at 1
- **recommendations_seq:** Starts at 1

#### 3. Table Creation
Tables are created to store data for the online shopping system with appropriate constraints and foreign key relationships:
- **Customers:** Stores customer information with a unique email constraint.
- **Productcategories:** Stores product categories with a primary key.
- **Products:** Stores product details with a foreign key to product categories.
- **Orders:** Stores order details with foreign keys to customers and products.
- **Creditcards:** Stores credit card details with a composite primary key and a foreign key to customers.
- **Invoices:** Stores invoice details with foreign keys to orders, customers, and credit cards.
- **Reviews:** Stores product reviews with a foreign key to products.
- **Recommendations:** Stores product recommendations with foreign keys to customers and products.

#### 4. Data Insertion
Sample data is inserted into each table using the created sequences to generate unique identifiers:
- **Customers:** Multiple rows of customer data with unique email addresses.
- **Productcategories:** Multiple rows of product category data.
- **Products:** Multiple rows of product data linked to categories.
- **Orders:** Multiple rows of order data linked to customers and products.
- **Creditcards:** Multiple rows of credit card data linked to customers.
- **Invoices:** Multiple rows of invoice data linked to orders, customers, and credit cards.
- **Reviews:** Multiple rows of review data linked to products.
- **Recommendations:** Multiple rows of recommendation data linked to customers and products.

#### 5. Example Queries
The script concludes with queries to retrieve and display all data from the created tables, allowing verification of the inserted data and the relationships between different entities.

### Conclusion
This SQL script provides a comprehensive setup for an online shopping database system, including schema definition, relationship management, and data population. It ensures that all necessary components are in place for efficient database operations and data integrity in an e-commerce environment.
