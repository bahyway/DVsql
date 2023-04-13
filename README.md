---
description: This is a Data Vault Documentations
---

# Data Vault

Data Vault is a modeling methodology for building data warehouses that emphasizes agility, scalability, and resilience. It is based on the principles of 3rd Normal Form, which is a standard approach to organizing data in a relational database.

In 3rd Normal Form, data is organized into multiple related tables, with each table containing a unique set of attributes. The relationships between tables are defined using foreign keys, which enable the retrieval of related data across multiple tables.

Data Vault extends the principles of 3rd Normal Form by introducing the concepts of Hubs, Links, and Satellites. Hubs are tables that contain a unique list of natural keys (also known as business keys) for a particular entity. Links are tables that represent the relationships between entities, using the natural keys from their respective Hubs. Satellites are tables that contain additional descriptive or historical information about an entity or relationship.

In Data Vault, all attributes are stored in Satellites, and the natural keys are stored in Hubs and Links. This approach allows for maximum flexibility and scalability, as changes to the attributes or relationships can be easily accommodated without requiring a complete redesign of the data model.

Data Vault also emphasizes the use of Hash Keys, which are system-generated keys based on the values of the attributes of an entity. Hash Keys are used to linking entities together and provide a fast, efficient way to search and retrieve data from the data warehouse.

In summary, Data Vault is a modeling methodology for building data warehouses that extends the principles of 3rd Normal Form by introducing the concepts of Hubs, Links, and Satellites. It emphasizes the use of natural keys and Hash Keys to enable maximum flexibility, scalability, and resilience in the data warehouse.
