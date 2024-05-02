# PALELC
- An extension of CAP.
- States that in the case of network partition (P) a distributed system can have trade-offs between availability (A) and consistency (C) else (E) if there is no network partition then a distributed system can have trade-offs between latency (L) and consistency (C).

<div align="center">
    <img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*oyXj3rXh8Rx2Uxm8-M3LrQ@2x.jpeg". width=70%>
</div>

# CAP vs. PALELC
- **CAP**
    - In the case of network partitioning in a distributed system, one has to choose between availability and Consistency.
    - Does not provide trade-offs when the system is under normal functioning or non-partitioned.
    - Cannot answer about what happens when there is no partition or what logical combination then a distributed system have.
- **PALELC**
    - Extends CAP by introducing latency as an additional attribute of a distributed system.
    - Developed to address a key limitation of CAP as it makes no provision for performance or latency.

# Features of PALELC
- **PAC**
    - Same as CAP.
- **ELC**
    - Low latancy and eventual consistency.
    - Strong Consistency and high latancy.
