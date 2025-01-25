# Dirty Read Phenomena

One transaction may read a data that another transaction never committed.

Example:

- Transaction A changed some data.
- Transaction B read that data.
- Transaction A rollbacks.
- Transaction B do something with data.
- Transaction B commits.

The data committed from transaction B it's based on some data that never actually existed on the database.

###### Tags

#database #sql #readphenomena #dirtyread