# BASE
- A set of principles that guide the design and operation of modern databases. 

# Concepts of BASE
- **Basically Available**
    - A distributed system should be available to respond with some acknowledgment even if it’s a failure message, to any incoming request.
- **Soft State**
    - The system may keep changing states as and when it receives new information.
- **Eventually Consistent**
    - The components in the system may not reflect the same value and state of a record at a given point in time.
    - They will settle it with time, eventually.
 
# ACID vs. BASE
- **ACID**
    - Requires immediate consistency.
    - Better suited to traditional transactional databases.
- **BASE**
    - Requires eventual consistency.
    - More suitable for use in large-scale, highly-available systems.
