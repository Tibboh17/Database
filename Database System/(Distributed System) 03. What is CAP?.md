# CAP
- A theorem states that a distributed system can deliver only two of three desired characteristics.

# Concepts of CAP
- **Consistency**
    - All the replicas that have a particular record must return the exact same value.
- **Availability**
    - All the active nodes at any moment must be able to respond to different operations.
- **Partition Tolerance**
    - The system must be able to tolerate network partition among its participant nodes.

<div align="center">
    <img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*2ths6CluMGCcNcSFLkFzag.png", width=50%>
</div>

# Features of CAP
- **CA**
    - Consistency and Availability
    - Maintains strong data consistency and high responsiveness but sacrifices Partition Tolerance.
    - Works well in stable network conditions, but it may become problematic during network partitions.
- **AP**
    - Availability and Partition Tolerance
    - Aims for high system availability and the ability to operate under network partitions.
    - Comes at the cost of relaxing strong consistency, allowing for temporary data inconsistencies.
- **CP**
    - Consistency and Partition Tolerance
    - Ensures strong data consistency and the ability to withstand network partitions.
    - Results in periods of unavailability during partition events.
