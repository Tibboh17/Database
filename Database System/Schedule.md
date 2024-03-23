# Schedule
- A process of lining the transactions and executing them one by one for maintaining consistency of the database.

# Types of Schedule
- **Serial Schedule**
    - The transactions are executed non-interleaved.
    - No transaction starts until a running transaction has ended.
- **Non-Serial Schedule**
    - The operations of multiple transactions are interleaved.
    - The other transaction proceeds without waiting for the previous transaction to complete.
 
<div align="center">
    <img src="https://scaler.com/topics/images/types-of-schedules.webp", width=70%>
</div>

<div align="center">
    <img src="https://scaler.com/topics/images/serial%20vs%20serializable.webp", width=70%>
</div>

# Conflict Serializable
- A schedule which can be transformed into a serial schedule by swapping non-conflicting operations.
- Two operations are said to be conflicting if all conditions satisfy the conditions below.
    - They belong to different transactions.
    - They operate on the same data item.
    - At least one of them is a write operation.
 
<div align="center">
    <img src="https://scaler.com/topics/images/conflict-serializability.webp", width=70%>
</div>

# View Serializable
- A Schedule which is view equal to a serial schedule.
- If a schedule is conflict serializable, then it will be view serializable.
- The view serializable which does not conflict with serializable, contains blind writes.

<div align="center">
    <img src="https://scaler.com/topics/images/view-serializability.webp", width=70%>
</div>

# Recoverable Schedule
- A schedule is recoverable if each transaction commits only after all the transactions from which it has read have committed.
- If some transaction T2 reads a value that has been updated/written by some other transaction T1, then the commit of T2 must occur after the commit of T1.

<div align="center">
    <img src="https://scaler.com/topics/images/recoverable-schedule.webp", width=70%>
</div>

# Cascading Schedule
- A schedule that several other dependent transactions are forced to rollback/abort because of the failure of one transaction.
- If some transactions had been committed before the failure of their previous transaction, then the schedule would have been irrecoverable.

<div align="center">
    <img src="https://scaler.com/topics/images/cascading-schedule.webp", width=70%>
</div>

# Cascadless
- A schedule that a transaction is not allowed to read a data item until and unless the last transaction that has been written is committed/aborted.
- To prevent cascading rollbacks, it disallows a transaction from reading uncommitted changes from another transaction in the same schedule.
- If some transaction T2 wants to read a value that has been updated or written by some other transaction T1, then only after the commit of T1, the commit of T2 must read it.

<div align="center">
    <img src="https://scaler.com/topics/images/cascadeless-schedule.webp", width=70%>
</div>

# Non-Recoverable Schedule
- A schedule that a transaction reads the value of an operation from an uncommitted transaction and commits before the transaction from where it has read the value.
- If there is a system failure, we may not be able to recover to a consistent database state.

<div align="center">
    <img src="https://scaler.com/topics/images/non-recoverable-schedule.webp", width=70%>
</div>
