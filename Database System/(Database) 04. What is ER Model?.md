# ER Model
- Entity-Relation Model.
- Represents a logical view of the system from a data perspective.

<div align="center">
    <img src="https://scaler.com/topics/images/what-is-er-model-in-dbms.webp", width="70%">
</div>

# Concepts of ER Model
- **Entity**
    - An object with a physical existence or an object with a conceptual existence.
- **Attribute**
    - The characteristics or properties which define the entity type. 
- **Relationship**
    - The association between entity types.
 
# Concepts of Entity
- **Entity Set**
    - A group of entities of similar kinds.
    - Contains entities with attributes that share similar values.
- **Strong Entity**
    - An entity type that has a key attribute.
    - Doesn't depend on other entities in the schema.
    - Represented by a single rectangle in ER diagram.
- **Weak Entity**
    - An entity type that doesn’t have a key attribute.
    - Cannot be uniquely identified by its attributes alone.
    - Represented by a double-outlined rectangle in ER diagrams.
 
# Concepts of Attribute
- **Simple Attribute**
    - Key attribute.
    - An attribute that cannot be further decomposed into sub-attributes.
    - Represented by an oval with a underlying line in ER diagram.
- **Composit Attribute**
    - An attribute that is composed of many other attributes and can be decomposed into simple attributes.
    - Represented by an oval comprising of ovals in ER diagram.
- **Multivalued Attribute**
    - An attribute that can have more that ont value.
    - Represented by a double oval in ER diagram.
- **Derived Attribute**
    - An attribute that can be derived from other attributes of an enity type.
    - Represented by a dashed oval in ER diagram.

<div align="center">
    <img src="https://scaler.com/topics/images/complete-student-entity-type-having-different-types-of-attributes.webp", width="70%">
</div>
 
# Concepts of Relationship
- **One-to-One**
    - Only one instance of an entity is associated with the relationship to one instance of another entity.
 
<div align="center">
    <img src="https://scaler.com/topics/images/one-to-one-relationship.webp", width="70%">
</div>

- **One-to-Many**
    - Only one instance of the entity on the left side of the relationship is linked to multiple instances of the entity on the right side.
 
<div align="center">
    <img src="https://scaler.com/topics/images/one-to-many-relationship.webp", width="70%">
</div>

- **Many-to-One**
    - Multiple instances of the entity on the left side of the relationship are linked to only one instance of the entity on the right side.

<div align="center">
    <img src="https://scaler.com/topics/images/many-to-one-relationships.webp", width="70%">
</div>

- **Many-to-Many**
    - Multiple instances of the entity on the left side of the relationship are to multiple instances of the entity on the right side.

<div align="center">
    <img src="https://scaler.com/topics/images/many-to-many-relationship.webp", width="70%">
</div>
