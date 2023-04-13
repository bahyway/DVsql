# Insert-Only Architecture

In Data Vault, the "Insert-Only Architecture" refers to the approach of only inserting data into the data warehouse, never updating or deleting it. This approach ensures that the data warehouse remains a complete and accurate record of all the data that has been loaded into it, making it ideal for auditing and compliance purposes.

The Insert-Only Architecture is achieved through the use of Satellites, which are tables that contain historical or descriptive information about an entity or relationship. Each Satellite contains a timestamp indicating when the record was created, as well as any subsequent changes that have been made to it. When a new record is inserted into the data warehouse, a new row is created in the corresponding Satellite, rather than updating an existing row.

This approach has several advantages:

1. Complete and Accurate History: By only inserting data into the data warehouse, the Insert-Only Architecture ensures that the data warehouse contains a complete and accurate record of all the data that has been loaded into it, including historical changes.
2. Simplified ETL Processes: Because data is only inserted into the data warehouse, rather than updated or deleted, ETL (Extract, Transform, Load) processes can be simplified, as there is no need to track or handle updates or deletions.
3. Improved Performance: By eliminating the need for updates and deletes, the Insert-Only Architecture can improve the performance of the data warehouse, as there are fewer locks and less contention for resources.
4. Enhanced Auditing and Compliance: Because the data warehouse contains a complete and accurate record of all the data that has been loaded into it, it is ideal for auditing and compliance purposes.

In summary, Data Vault's Insert-Only Architecture is an approach to building a data warehouse that emphasizes the insertion of data only, and never updating or deleting it. This approach is achieved through the use of Satellites, which contain historical or descriptive information about an entity or relationship. The Insert-Only Architecture ensures a complete and accurate record of all data loaded into the data warehouse, simplifies ETL processes, improves performance, and enhances auditing and compliance.
