# Database Schema Design Prompt

This prompt is designed to help you provide all the necessary information for designing a database schema.

Please fill in the following sections with as much detail as possible:

## 1. Application Overview

*   **Brief Description:** Describe the purpose and main functionalities of the application that will use this database.
*   **Core Features:** What are the most important features that rely on data storage?

## 2. Key Entities & Relationships

*   **Entities:** List the main entities (e.g., User, Product, Order, Post, Comment) that will be stored in the database.
*   **Relationships:** For each pair of related entities, describe the relationship (e.g., One-to-One, One-to-Many, Many-to-Many) and any specific rules (e.g., "A User can have many Orders, but an Order belongs to only one User").

## 3. Data Attributes for Each Entity

For each entity listed above, provide the following details:

*   **Entity Name:**
    *   **Attribute Name:** `Data Type` (e.g., `VARCHAR(255)`, `INT`, `BOOLEAN`, `DATETIME`, `DECIMAL(10,2)`)
    *   **Description:** (e.g., "Unique identifier for the user", "User's email address", "Price of the product")
    *   **Constraints:** (e.g., `PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`, `DEFAULT value`)

    *Example:*
    *   **Entity Name: User**
        *   `id`: `INT` (PRIMARY KEY, AUTO_INCREMENT)
        *   `username`: `VARCHAR(50)` (UNIQUE, NOT NULL)
        *   `email`: `VARCHAR(100)` (UNIQUE, NOT NULL)
        *   `created_at`: `DATETIME` (NOT NULL, DEFAULT CURRENT_TIMESTAMP)

## 4. Constraints & Business Rules

*   **Uniqueness:** Are there any attributes or combinations of attributes that must be unique (besides primary keys)?
*   **Validation Rules:** Are there any specific validation rules for data (e.g., "email must be a valid email format", "age must be greater than 18")?
*   **Referential Integrity:** Any specific rules for how related data should behave on deletion or update (e.g., CASCADE, SET NULL, RESTRICT)?

## 5. Expected Data Volume & Performance

*   **Estimated Number of Records:** Provide a rough estimate for the number of records for each entity (e.g., "Users: 1 million", "Orders: 10 million per year").
*   **Read/Write Frequency:** Which entities will be read from or written to most frequently?
*   **Performance Expectations:** Are there any specific performance requirements (e.g., "User login must be under 100ms", "Product search must be real-time")?

## 6. Preferred Database System (Optional)

*   Do you have a preferred database system (e.g., PostgreSQL, MySQL, MongoDB, SQLite, SQL Server, Convex, Firebase, Supabase)? If so, why?

## 7. Example Data (Optional)

*   Provide a few rows of example data for each key entity to illustrate the data structure and relationships.

## 8. Desired Output Format

*   What kind of output would you prefer for the database schema? (e.g., ER Diagram, SQL DDL statements, JSON schema, textual description, a combination of these)