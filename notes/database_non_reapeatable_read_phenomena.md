# Non Repeatable Read Phenomena

When a transaction select the same row twice but at the second time it get's different values.

Example:

- Transaction A select row with id 1;
- Transaction B update some value of row with id 1;
-  Transaction B commits (or not, depending on the isolation levels);
- Transaction A select row with id 1 again;

###### Tags

#database #sql #readphenomena #nonrepeatableread