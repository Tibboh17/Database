# Relational Model
- Represents how data is stored in Relational Databases.
- Uses a collection of tables to represent both data and the relationships among those data.
<div align="center">
  <img src="https://github.com/TIBBOH17/Database/assets/121493257/57f1a3c0-f686-4076-8412-34a2c84979dd" width="50%">
</div>

# Features of Relational Model
- Tuple has no duplicate value.
- Order of tuple can have a difference sequence.
- Attribute domain has no significance.
- Each attribute contains a distinct name.
- Each relation cell contains exactly one atomic (single) value.
- Name of the relation is distinct from all other relations.

# Concepts of Ralational Model
- **Attribute**
    - The properties which define a relation.
- **Column**
    - The set of values for a specific attribute.
- **Tuple**
    - Each row in the relation.
- **Relation Schema**
    - The name of the relation with its attributes.
- **Relation Instance**
    - A finite set of tuples in RDBMS.
- **Relation Key**
    - Used to identify the rows uniquely or also help in identifying tables.
- **Degree**
    - The total number of attributes which in the relation.
- **Cardinality**
    - The total number of rows which in the Table.
- **NULL Values**
    - The value which is not known or unavailable.
 
# Constraints in Relational Model
- **Domain Constraint**
    - Every domain must contain atomic values.
- **Entity Integrity Constraint**
    - No primary key can take a NULL value.
- **Referential Integrity Constraint**
    - If a given relation refers to a key attribute of a different or same table, then that key must exist in the given relation.
- **Key Constraint (Uniqueness Constraint)**
    - Every tuple in the relation should be unique.
