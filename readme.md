```
 
 migrate create -ext sql -dir migrations mango_sku_attribute_id_to_bigserial

localhost:  
 migrate -source file://./migrations  -database postgres://postgres:postgres@127.0.0.1:5432/vdev?sslmode=disable up 1
 
```
- **4. SQL Syntax**
   - [4.1. Lexical Structure](./postgresql/migrations/20200815134218_create_sponsor.up.sql)
   - [4.2. Value Expressions | type cast](postgresql/migrations/20200815134218_create_sponsor.up.sql)
- **5. Data Definition**
   - [5.1. Table Basics](./postgresql/migrations/20200815143131_create_showcase_rule.up.sql)
   - [5.2. Default Values](./postgresql/migrations/20200815143131_create_showcase_rule.up.sql)
   - [5.3. Constraints](./postgresql/migrations/20200815143131_create_showcase_rule.up.sql)
   - [5.5. Modifying Tables](./postgresql/migrations/20200815100413_alter_users_add_foreign_key.up.sql)
   - [5.7. Schemas](./postgresql/migrations/20200815143131_create_showcase_rule.up.sql)
   - [5.9. Table Partitioning](./postgresql/migrations/20200816080623_create_user_log.up.sql) | [insert | query](./postgresql/data_manipulation/user_log_inserting_data.sql)
   - [5.10. Other Database Objects]()
   - [5.11. Dependency Tracking]()
- **6. Data Manipulation**
   - [6.1. Inserting Data](./postgresql/data_manipulation/user_log_inserting_data.sql)
   - [6.2. Updating Data](./postgresql/data_manipulation/user_log_inserting_data.sql)
   - [6.3. Deleting Data](./postgresql/data_manipulation/order_insert_update_query.sql)
   - [6.4. Returning Data From Modified Rows]()
- **7. Queries**
   - [7.1. Overview]()
   - [7.2. Table Expressions]()
   - [7.3. Select Lists]()
   - [7.4. Combining Queries]()
   - [7.5. Sorting Rows]()
   - [7.6. LIMIT and OFFSET]()
   - [7.7. VALUES Lists]()
   - [7.8. WITH Queries (Common Table Expressions)](./postgresql/data_manipulation/projects_insert_data.sql)
- **8. Data Types**
   - [8.1. Numeric Types | int2,int4,int8 | real,double precision | smallserial, serial, bigserial](postgresql/migrations/20200815134218_create_sponsor.up.sql)
   - [8.2. Monetary Types]()
   - [8.3. Character Types | varchar | char | text](./postgresql/migrations/20200814135132_create_user.up.sql)
   - [8.4. Binary Data Types]()
   - [8.5. Date/Time Types](./postgresql/migrations/20200814135132_create_user.up.sql)
   - [8.6. Boolean Type | true | yes | on | 1]()
   - [8.7. Enumerated Types | order | type safety](postgresql/migrations/20200815121818_create_type_pushstatus.up.sql)
   - [8.8. Geometric Types | point | lines | boxes | polygons | circle]()
   - [8.9. Network Address Types]()
   - [8.10. Bit String Types todo]()
   - [8.11. Text Search Types todo]()
   - [8.12. UUID Type](./postgresql/migrations/20200814135132_create_user.up.sql)
   - [8.13. XML Type todo]()
   - [8.14. JSON Types | input output syntax | reparse ](postgresql/migrations/20200815134218_create_sponsor.up.sql)
   - [8.14. JSONB Types | binary | gin indexing](postgresql/migrations/20200817163700_create_orders.up.sql)
   - [8.15. Arrays | input output syntax | accessing | modify | search  ](./postgresql/migrations/20200817163700_create_orders.up.sql)
   - [8.16. Composite Types]()
   - [8.17. Range Types | input output syntax | GiST and SP-GiST index](postgresql/migrations/20200815143131_create_showcase_rule.up.sql)
   - [8.18. Domain Types todo]()
   - [8.19. Object Identifier Types todo]()
   - [8.20. pg_lsn Type todo]()
   - [8.21. Pseudo-Types todo]()
- **9. Functions and Operators**
   - [9.1. Logical Operators]()
   - [9.2. Comparison Functions and Operators]()
   - [9.3. Mathematical Functions and Operators]()
   - [9.4. String Functions and Operators]()
   - [9.5. Binary String Functions and Operators]()
   - [9.6. Bit String Functions and Operators]()
   - [9.7. Pattern Matching]()
   - [9.8. Data Type Formatting Functions]()
   - [9.9. Date/Time Functions and Operators]()
   - [9.10. Enum Support Functions]()
   - [9.11. Geometric Functions and Operators]()
   - [9.12. Network Address Functions and Operators]()
   - [9.13. Text Search Functions and Operators]()
   - [9.14. XML Functions]()
   - [9.15. JSON Functions and Operators]()
   - [9.16. Sequence Manipulation Functions]()
   - [9.17. Conditional Expressions]()
   - [9.18. Array Functions and Operators]()
   - [9.19. Range Functions and Operators]()
   - [9.20. Aggregate Functions]()
   - [9.21. Window Functions]()
   - [9.22. Subquery Expressions]()
   - [9.23. Row and Array Comparisons]()
   - [9.24. Set Returning Functions]()
   - [9.25. System Information Functions and Operators]()
   - [9.26. System Administration Functions]()
   - [9.27. Trigger Functions]()
   - [9.28. Event Trigger Functions]()
   - [9.29. Statistics Information Functions]()
- **10. Type Conversion**
   - [10.1. Overview]()
   - [10.2. Operators]()
   - [10.3. Functions]()
   - [10.4. Value Storage]()
   - [10.5. UNION, CASE, and Related Constructs]()
- **11. Indexes**
   - [11.1. Introduction]()
   - [11.2. Index Types]()
   - [11.3. Multicolumn Indexes]()
   - [11.4. Indexes and ORDER BY]()
   - [11.5. Combining Multiple Indexes]()
   - [11.6. Unique Indexes]()
   - [11.7. Indexes on Expressions]()
   - [11.8. Partial Indexes]()
   - [11.9. Index-Only Scans and Covering Indexes]()
   - [11.10. Operator Classes and Operator Families]()
   - [11.11. Indexes and Collations]()
   - [11.12. Examining Index Usage]()
- **12. Full Text Search**
   - [12.1. Introduction]()
   - [12.2. Tables and Indexes]()
   - [12.3. Controlling Text Search]()
   - [12.4. Additional Features]()
   - [12.5. Parsers]()
   - [12.6. Dictionaries]()
   - [12.7. Configuration Example]()
   - [12.8. Testing and Debugging Text Search]()
   - [12.9. GIN and GiST Index Types]()
   - [12.10. psql Support]()
   - [12.11. Limitations]()
- **13. Concurrency Control**
   - [13.1. Introduction]()
   - [13.2. Transaction Isolation]()
   - [13.3. Explicit Locking]()
   - [13.4. Data Consistency Checks at the Application Level]()
   - [13.5. Caveats]()
   - [13.6. Locking and Indexes]()
- **14. Performance Tips**
   - [14.1. Using EXPLAIN]()
   - [14.2. Statistics Used by the Planner]()
   - [14.3. Controlling the Planner with Explicit JOIN Clauses]()
   - [14.4. Populating a Database]()
   - [14.5. Non-Durable Settings]()
- **I. SQL Commands**
   - [ABORT — abort the current transaction]()
   - [ALTER AGGREGATE — change the definition of an aggregate function]()
   - [ALTER COLLATION — change the definition of a collation]()
   - [ALTER CONVERSION — change the definition of a conversion]()
   - [ALTER DATABASE — change a database]()
   - [ALTER DEFAULT PRIVILEGES — define default access privileges]()
   - [ALTER DOMAIN — change the definition of a domain]()
   - [ALTER EVENT TRIGGER — change the definition of an event trigger]()
   - [ALTER EXTENSION — change the definition of an extension]()
   - [ALTER FOREIGN DATA WRAPPER — change the definition of a foreign-data wrapper]()
   - [ALTER FOREIGN TABLE — change the definition of a foreign table]()
   - [ALTER FUNCTION — change the definition of a function]()
   - [ALTER GROUP — change role name or membership]()
   - [ALTER INDEX — change the definition of an index]()
   - [ALTER LANGUAGE — change the definition of a procedural language]()
   - [ALTER LARGE OBJECT — change the definition of a large object]()
   - [ALTER MATERIALIZED VIEW — change the definition of a materialized view]()
   - [ALTER OPERATOR — change the definition of an operator]()
   - [ALTER OPERATOR CLASS — change the definition of an operator class]()
   - [ALTER OPERATOR FAMILY — change the definition of an operator family]()
   - [ALTER POLICY — change the definition of a row level security policy]()
   - [ALTER PROCEDURE — change the definition of a procedure]()
   - [ALTER PUBLICATION — change the definition of a publication]()
   - [ALTER ROLE — change a database role]()
   - [ALTER ROUTINE — change the definition of a routine]()
   - [ALTER RULE — change the definition of a rule]()
   - [ALTER SCHEMA — change the definition of a schema]()
   - [ALTER SEQUENCE — change the definition of a sequence generator]()
   - [ALTER SERVER — change the definition of a foreign server]()
   - [ALTER STATISTICS — change the definition of an extended statistics object]()
   - [ALTER SUBSCRIPTION — change the definition of a subscription]()
   - [ALTER SYSTEM — change a server configuration parameter]()
   - [ALTER TABLE — change the definition of a table](./postgresql/migrations/20200815100413_alter_users_add_foreign_key.up.sql)
   - [ALTER TABLESPACE — change the definition of a tablespace]()
   - [ALTER TEXT SEARCH CONFIGURATION — change the definition of a text search configuration]()
   - [ALTER TEXT SEARCH DICTIONARY — change the definition of a text search dictionary]()
   - [ALTER TEXT SEARCH PARSER — change the definition of a text search parser]()
   - [ALTER TEXT SEARCH TEMPLATE — change the definition of a text search template]()
   - [ALTER TRIGGER — change the definition of a trigger]()
   - [ALTER TYPE — change the definition of a type](postgresql/migrations/20200815130436_alter_type_pushstatus.up.sql)
   - [ALTER USER — change a database role]()
   - [ALTER USER MAPPING — change the definition of a user mapping]()
   - [ALTER VIEW — change the definition of a view]()
   - [ANALYZE — collect statistics about a database]()
   - [BEGIN — start a transaction block]()
   - [CALL — invoke a procedure]()
   - [CHECKPOINT — force a write-ahead log checkpoint]()
   - [CLOSE — close a cursor]()
   - [CLUSTER — cluster a table according to an index]()
   - [COMMENT — define or change the comment of an object]()
   - [COMMIT — commit the current transaction]()
   - [COMMIT PREPARED — commit a transaction that was earlier prepared for two-phase commit]()
   - [COPY — copy data between a file and a table]()
   - [CREATE ACCESS METHOD — define a new access method]()
   - [CREATE AGGREGATE — define a new aggregate function]()
   - [CREATE CAST — define a new cast]()
   - [CREATE COLLATION — define a new collation]()
   - [CREATE CONVERSION — define a new encoding conversion]()
   - [CREATE DATABASE — create a new database]()
   - [CREATE DOMAIN — define a new domain]()
   - [CREATE EVENT TRIGGER — define a new event trigger]()
   - [CREATE EXTENSION — install an extension]()
   - [CREATE FOREIGN DATA WRAPPER — define a new foreign-data wrapper]()
   - [CREATE FOREIGN TABLE — define a new foreign table]()
   - [CREATE FUNCTION — define a new function](./postgresql/migrations/20200814135132_create_user.up.sql)
   - [CREATE GROUP — define a new database role]()
   - [CREATE INDEX — define a new index](./postgresql/migrations/20200815134218_create_sponsor.up.sql)
   - [CREATE LANGUAGE — define a new procedural language]()
   - [CREATE MATERIALIZED VIEW — define a new materialized view]()
   - [CREATE OPERATOR — define a new operator]()
   - [CREATE OPERATOR CLASS — define a new operator class]()
   - [CREATE OPERATOR FAMILY — define a new operator family]()
   - [CREATE POLICY — define a new row level security policy for a table]()
   - [CREATE PROCEDURE — define a new procedure]()
   - [CREATE PUBLICATION — define a new publication]()
   - [CREATE ROLE — define a new database role]()
   - [CREATE RULE — define a new rewrite rule]()
   - [CREATE SCHEMA — define a new schema]()
   - [CREATE SEQUENCE — define a new sequence generator]()
   - [CREATE SERVER — define a new foreign server]()
   - [CREATE STATISTICS — define extended statistics]()
   - [CREATE SUBSCRIPTION — define a new subscription]()
   - [CREATE TABLE — define a new table](./postgresql/migrations/20200815094424_create_emails.up.sql)
   - [CREATE TABLE AS — define a new table from the results of a query]()
   - [CREATE TABLESPACE — define a new tablespace]()
   - [CREATE TEXT SEARCH CONFIGURATION — define a new text search configuration]()
   - [CREATE TEXT SEARCH DICTIONARY — define a new text search dictionary]()
   - [CREATE TEXT SEARCH PARSER — define a new text search parser]()
   - [CREATE TEXT SEARCH TEMPLATE — define a new text search template]()
   - [CREATE TRANSFORM — define a new transform]()
   - [CREATE TRIGGER — define a new trigger](postgresql/migrations/20200814135132_create_user.up.sql)
   - [CREATE TYPE — define a new data type](postgresql/migrations/20200815121818_create_type_pushstatus.up.sql)
   - [CREATE USER — define a new database role]()
   - [CREATE USER MAPPING — define a new mapping of a user to a foreign server]()
   - [CREATE VIEW — define a new view]()
   - [DEALLOCATE — deallocate a prepared statement]()
   - [DECLARE — define a cursor]()
   - [DELETE — delete rows of a table]()
   - [DISCARD — discard session state]()
   - [DO — execute an anonymous code block]()
   - [DROP ACCESS METHOD — remove an access method]()
   - [DROP AGGREGATE — remove an aggregate function]()
   - [DROP CAST — remove a cast]()
   - [DROP COLLATION — remove a collation]()
   - [DROP CONVERSION — remove a conversion]()
   - [DROP DATABASE — remove a database]()
   - [DROP DOMAIN — remove a domain]()
   - [DROP EVENT TRIGGER — remove an event trigger]()
   - [DROP EXTENSION — remove an extension]()
   - [DROP FOREIGN DATA WRAPPER — remove a foreign-data wrapper]()
   - [DROP FOREIGN TABLE — remove a foreign table]()
   - [DROP FUNCTION — remove a function]()
   - [DROP GROUP — remove a database role]()
   - [DROP INDEX — remove an index]()
   - [DROP LANGUAGE — remove a procedural language]()
   - [DROP MATERIALIZED VIEW — remove a materialized view]()
   - [DROP OPERATOR — remove an operator]()
   - [DROP OPERATOR CLASS — remove an operator class]()
   - [DROP OPERATOR FAMILY — remove an operator family]()
   - [DROP OWNED — remove database objects owned by a database role]()
   - [DROP POLICY — remove a row level security policy from a table]()
   - [DROP PROCEDURE — remove a procedure]()
   - [DROP PUBLICATION — remove a publication]()
   - [DROP ROLE — remove a database role]()
   - [DROP ROUTINE — remove a routine]()
   - [DROP RULE — remove a rewrite rule]()
   - [DROP SCHEMA — remove a schema]()
   - [DROP SEQUENCE — remove a sequence]()
   - [DROP SERVER — remove a foreign server descriptor]()
   - [DROP STATISTICS — remove extended statistics]()
   - [DROP SUBSCRIPTION — remove a subscription]()
   - [DROP TABLE — remove a table]()
   - [DROP TABLESPACE — remove a tablespace]()
   - [DROP TEXT SEARCH CONFIGURATION — remove a text search configuration]()
   - [DROP TEXT SEARCH DICTIONARY — remove a text search dictionary]()
   - [DROP TEXT SEARCH PARSER — remove a text search parser]()
   - [DROP TEXT SEARCH TEMPLATE — remove a text search template]()
   - [DROP TRANSFORM — remove a transform]()
   - [DROP TRIGGER — remove a trigger]()
   - [DROP TYPE — remove a data type]()
   - [DROP USER — remove a database role]()
   - [DROP USER MAPPING — remove a user mapping for a foreign server]()
   - [DROP VIEW — remove a view]()
   - [END — commit the current transaction]()
   - [EXECUTE — execute a prepared statement]()
   - [EXPLAIN — show the execution plan of a statement]()
   - [FETCH — retrieve rows from a query using a cursor]()
   - [GRANT — define access privileges]()
   - [IMPORT FOREIGN SCHEMA — import table definitions from a foreign server]()
   - [INSERT — create new rows in a table]()
   - [LISTEN — listen for a notification]()
   - [LOAD — load a shared library file]()
   - [LOCK — lock a table]()
   - [MOVE — position a cursor]()
   - [NOTIFY — generate a notification]()
   - [PREPARE — prepare a statement for execution]()
   - [PREPARE TRANSACTION — prepare the current transaction for two-phase commit]()
   - [REASSIGN OWNED — change the ownership of database objects owned by a database role]()
   - [REFRESH MATERIALIZED VIEW — replace the contents of a materialized view]()
   - [REINDEX — rebuild indexes]()
   - [RELEASE SAVEPOINT — destroy a previously defined savepoint]()
   - [RESET — restore the value of a run-time parameter to the default value]()
   - [REVOKE — remove access privileges]()
   - [ROLLBACK — abort the current transaction]()
   - [ROLLBACK PREPARED — cancel a transaction that was earlier prepared for two-phase commit]()
   - [ROLLBACK TO SAVEPOINT — roll back to a savepoint]()
   - [SAVEPOINT — define a new savepoint within the current transaction]()
   - [SECURITY LABEL — define or change a security label applied to an object]()
   - [SELECT — retrieve rows from a table or view]()
   - [SELECT INTO — define a new table from the results of a query]()
   - [SET — change a run-time parameter]()
   - [SET CONSTRAINTS — set constraint check timing for the current transaction]()
   - [SET ROLE — set the current user identifier of the current session]()
   - [SET SESSION AUTHORIZATION — set the session user identifier and the current user identifier of the current session]()
   - [SET TRANSACTION — set the characteristics of the current transaction]()
   - [SHOW — show the value of a run-time parameter]()
   - [START TRANSACTION — start a transaction block]()
   - [TRUNCATE — empty a table or set of tables]()
   - [UNLISTEN — stop listening for a notification]()
   - [UPDATE — update rows of a table]()
   - [VACUUM — garbage-collect and optionally analyze a database]()
   - [VALUES — compute a set of rows](./postgresql/data_manipulation/emails_insert_data.sql)