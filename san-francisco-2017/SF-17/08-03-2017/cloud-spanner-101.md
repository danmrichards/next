# Cloud Spanner 101
## History
2005 - Everything on sharded clustered databases. A re-shard took years to complete.

## Google Needs
* Horizontally scaling database
* ACID transactions with global consistency
* No downtime
    * A minute of downtime on adwords cost millions of dollars

## What is Cloud Spanner
Mission critical scaleable RDBMS.

* Fully managed. Global scale
* Traditional relational semantics: schemas, ACID transactions, SQL
* Automatic, synchronous replication withing and across availability regions
* Battle-tested within Google for 5+ years (adwords, google play)

## Open Standards
* Standard SQL (ANSI 2011)
* Encryption, audit logging, identity and access management
* Client libraries in popular languages (Java, Python, Go, Node.js etc)
* JBDC driver

## Types of Workloads
* Transactional
    * Companies that have outgrown traditional RDBMS and have moved to NoSQL, but need transactional consistency
* Scale-out
    * Companies currently sharding database because they need more read/write throughput than can be placed on 1 node
* Global data plane
    * Companies and/or developers building applications that have global data and need strong consistency
* Database consolidation
    * Companies that store their business data in multiple database products with variable maintenance overheads

## Interleave Tables
* Store tables 'interleaved' with each other for common data
* Allows spanner to know to keep related data together in the same nodes
* Reduces need for 2-phase commit
* Create 1st table (`CREATE TABLE Singers...`) and interleave second table (`CREATE TABLE Albums...INTERLEAVE IN Singers;`)

## Demo
* Force use of indexes in a query (`FROM TableName@{FORCE_INDEX=IndexName}`)
* Monitoring metrics available from Spanner in Stackdriver
