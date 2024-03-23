# Log
- A sequence of records, which maintains the records of actions performed by a transaction.
- It is important that the logs are written prior to the actual modification and stored on a stable storage media, which is failsafe.

# Concepts of Log
- **[start_transaction, T]**
    - The start of execution of transaction T.
- **[write_item, T, X, old_value, new_value]**
    - The value of the variable, **X** is changed from **old_value** to **new_value** by the transaction **T**.
- **[read_item, T, X]**
    - The value of **X** is read by the transaction **T**.
- **[commit, T]**
    - The changes in the data are stored in the database through a **commit** and can't be further modified by the transaction.
    - There will be no error after a **commit** has been made to the database.
- **[abort, T]**
    - The transaction **T** is aborted.

# Undo
- Examine **[write_item, T, X, old_value, new_value]** operation and retirieve the state of data to **old_data**.
- Undo the changes made by the transactions with **[start_transaction, T]** but no **[commit, T]** or **[abort, T]**.

# Redo
- Convert the old state of data to the new state that was lost due to system failure.
- Redo the transactions with **[start_transaction, T]** and **[commit, T]**.

# Checkpoint
- Made after all the records of a transaction are written to logs.
- Transfer all the logs from the local storage to the permanent storage for future use.

<div align="center">
    <img src="https://scaler.com/topics/images/multiple-transaction.webp", width=70%>
</div>
