# Distributed-System-survey
## Summary:
This is a survey/notes of Distributed system/articles as reference for myself.

## OLTP:

  ### Hash Index/SSTable/LSM-tree

  ### B-Trees

  ### Optimization:
    * Bloom Filter: a data structure used to quickly check if a record exists in the database rather than exhaustive search for a non-existing database.


## OLAP
Online Analytic Processing is the term for describing the access pattern for data analytics. 
Example of queries are:
 * Monthly sales
 * Average salary
 
For small companies, these types of query are run on the same database as OLTP, which to some extent can be handled by transactional DB.
However the larger the dataset, the need for a dedicated OLAP system (Data Warehouse) emerges. These DB are optimized for these specific queries.

E.g: 
* ParAccell: http://www.dbms2.com/category/products-and-vendors/paraccel/
* Amazon RedShift
* SQL-on-Hadoop usually based on Google's Dremel: 
    * Apache Hive
    * Spark SQL
    * Cloudera Impala
    * Facebook Presto
    * Apache Tajo
    * Apache Drill

## Ref
* Design Data-Intensive Applications - Martin Kleppmann
* Principles of Distributed Database Systems - Özsu, M. Tamer, Valduriez, Patrick
* Dremel: Interactive Analysis of Web-Scale Datasets -https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36632.pdf
