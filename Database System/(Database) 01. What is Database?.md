# Database
- A collection of operational data that is integrated and stored so that it can be shared by multiple users in a specific organization.
- An organized collection of structured information, or data, typically stored electronically in a computer system.

# Database vs. Spreadsheet

#### Database
- Designed to hold much larger collections of organized information.
- Allows multiple users at the same time to quickly and securely access and query the data using highly complex logic and language.
- Supports ACID (Atomicity, Consistency, Isolation, Durability) properties to ensure reliable transactions.

#### Spreadsheet
- Originally designed for one user.
- Great for a single user or a small number of users who don’t need to do a lot of incredibly complicated data manipulation.
- Limited in terms of data capacity and collaboration features compared to databases.

# Concepts of Database

#### Database Schema
- A logical representation of data that shows how the data in a database should be stored logically.
- Includes definitions of tables, views, indexes, and other database objects.

#### Database Instance
- The data and information that is currently stored in the database at a specific point in time.

#### Data Constraints
- Rules enforced on data columns to ensure data integrity.
- Examples include primary key, foreign key, unique, not null, and check constraints.

#### Data Dictionary (Metadata)
- A collection of metadata such as object names, data types, sizes, classifications, and relationships with other data assets.
- Acts as a centralized repository of information about the database's data.

#### Data Manipulation
- Operations that modify the data in the database.
- Includes Insertion, Deletion, and Updation (Update).

#### Query
- A request to access data from the database to retrieve or manipulate it.
- Structured Query Language (SQL) is commonly used for querying relational databases.

# Types of Data
#### Structured Data
- Organized and easily searchable data, typically found in relational databases (e.g., tables with rows and columns).

#### Unstructured Data
- Data that lacks a predefined format or structure, such as text, images, and videos.

#### Semi-structured Data
- Data that does not conform to a rigid structure but has some organizational properties, such as JSON and XML.

# Types of Database
#### Hierarchical Database
- Data is organized in a tree-like structure. Each record has a single parent and multiple children.

#### Relational Database
- Uses tables (relations) to store data and establish relationships between them using keys. Examples include MySQL, PostgreSQL, and Oracle.

#### Non-relational Database
- Also known as NoSQL databases, they store data in a variety of ways other than tabular relations, such as document, key-value, graph, and column stores. Examples include MongoDB, Cassandra, and Neo4j.

# Three Level Architecture of Database

#### Physical Level
- Internal Level.
- Describes how data is actually stored in the database, including data structures and file organization.

#### Conceptual Level
- Logical Level.
- Describes how the database appears to users conceptually and the relationships between various data tables.
- Defines the logical structure of the entire database.

#### External Level
- View Level.
- Shows the relevant database content to the users in the form of views and hides the rest of the data.
- Provides multiple views of the database tailored to different users.
