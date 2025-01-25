# Phantom Read Phenomena

Some transaction make a query selecting based on some condition twice, at the second time it receives different rows.

Example:

- Transaction A select based on some condition and receives N rows;
- Transaction B change data that affect that condition;
- Transaction B commits (or not, depending on isolation level);
- Transaction A select again with same condition;

At the second time transaction A will receive different rows that previously.

###### Tags

#database #sql #readphenomena #phantomread