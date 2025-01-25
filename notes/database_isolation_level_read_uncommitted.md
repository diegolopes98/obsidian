# Read Uncommitted Isolation Level

Any data modification made by the transaction will be visible to others even if it didn't commit yet.

Example: 

- Transaction A starts
- Transaction B starts
- Transaction A change data
- Transaction B reads the same data transaction A changed
- Transaction A commits.

**Font:** 
- ByteByteGo System Design Big Archive
- Microsoft blog post (https://learn.microsoft.com/en-us/sql/connect/jdbc/understanding-isolation-levels?view=sql-server-2017)
###### Tags

#database #sql #isolationlevel #readuncommitted
