# Normalization
- The process of reducing data redundancy in a table and improving data integrity.

# Puposes of Normalization
- Reducing data redundancy or data duplication.
- Making a database more scalable without sacrificing performance.
- Simplfying the enforcement of integrity constraints.
- Preventing anomalies by making tables more logical and straigtforward.

# Anomalies
- **Insertion Anomaly**
    - Occurs when it is not possible to insert data into a database because the required fields are missing or the data is incomplete.
- **Update Anomaly**
    - Occurs when modifying data in a database can result in inconsisitencies or errors.
- **Deletion Anomaly**
    - Occurs when deleting a record can result in the unintentional loss of data.
 
# Funtional Dependency
- A fundamental concept that describes the relationship between attributes in a table.
- Normalize by analyzing functional dependencies.

# Inference Rule
- **Reflexive Rule**
    - If X ⊇ Y, then X → Y.
- **Augmentation Rule**
    - If X → Y, then XZ → YZ.
- **Transitive Rule**
    - If X → Y and Y → Z, then X → Z.    
- **Union Rule**
    - If X → Y and X → Z, then X → YZ.
- **Decomposotion Rule**
    - If X → YZ, then X → Y and X → Z.
- **Pseudo Transitive Rule**
    - If X → Y and YZ → W, then XZ → W.
 
# Data Normalization Forms
- **First Normal Form (1NF)**
    - Eliminate repeating groups in individual tables.
    - Create a seperate table for each set of related data.
    - Identify each set of related data with a primary key.
- **Second Normal Form (2NF)**
    - Create sperate tables for sets of values that apply to multiple records.
    - Relate these tables with a foreign key.
- **Third Normal Form (3NF)**
    - Eliminate fields that don't depend on the key.

# Other Normalization Forms
- **Boyce-Codd Normal Form (BCNF, 3.5NF)**
- **Fourth Normal Form (4NF)**
- **Fifth Normal Form (5NF)**
- **Sixth Normal Form (6NF)**

# Example of Normalization
- **Unnormalized table**

| **Student#** | **Advisor** | **Adv-Room** | **Class1** | **Class2** | **Class3** |
|:------------:|:-----------:|:------------:|:----------:|:----------:|:----------:|
|     1022     |    Jones    |      412     |   101-07   |   143-01   |   159-02   |
|     4123     |    Smith    |      216     |   101-07   |   143-01   |   179-04   |

- **First Normal Form**

| **Student#** | **Advisor** | **Adv-Room** | **Class#** |
|:------------:|:-----------:|:------------:|:----------:|
|     1022     |    Jones    |      412     |   101-07   |
|     1022     |    Jones    |      412     |   143-01   |
|     1022     |    Jones    |      412     |   159-02   |
|     4123     |    Smith    |      216     |   101-07   |
|     4123     |    Smith    |      216     |   143-01   |
|     4123     |    Smith    |      216     |   179-04   |

- **Second Normal Form**

| **Student#** | **Advisor** | **Adv-Room** |
|:------------:|:-----------:|:------------:|
|     1022     |    Jones    |      412     |
|     4123     |    Smith    |      216     |

| **Student#** | **Class#** |
|:------------:|:----------:|
|     1022     |   101-07   |
|     1022     |   143-01   |
|     1022     |   159-02   |
|     4123     |   101-07   |
|     4123     |   143-01   |
|     4123     |   179-04   |

- **Third Normal Form**
      
| **Student#** | **Advisor** |
|:------------:|:-----------:|
|     1022     |    Jones    |
|     4123     |    Smith    |

| **Student#** | **Class#** |
|:------------:|:----------:|
|     1022     |   101-07   |
|     1022     |   143-01   |
|     1022     |   159-02   |
|     4123     |   101-07   |
|     4123     |   143-01   |
|     4123     |   179-04   |

| **Name** | **Room** | **Dept** |
|:--------:|:--------:|:--------:|
|   Jones  |    412   |    42    |
|   Smith  |    216   |    42    |
