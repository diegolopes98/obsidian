# Read Committed Isolation Level

Any data modification made by the transaction will be visible to others only if it commits.

Example: 

- Transaction A starts
- Transaction B starts
- Transaction A change data
- Transaction B reads the data before transaction A changes it 
- Transaction A commits.
- Transaction B can now see transaction A changes.

**Font:** 
- ByteByteGo System Design Big Archive
- Microsoft blog post (https://learn.microsoft.com/en-us/sql/connect/jdbc/understanding-isolation-levels?view=sql-server-2017)

###### Tags

#database #sql #isolationlevel #readcommitted
