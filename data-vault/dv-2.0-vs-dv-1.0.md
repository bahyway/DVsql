# DV 2.0 vs DV 1.0

Data Vault is a modeling methodology for building data warehouses that emphasizes agility, scalability, and resilience. Data Vault 1.0 was introduced in the early 2000s and underwent several revisions, culminating in the release of Data Vault 2.0 in 2013. One of the key differences between the two versions is the use of a Hash Key.

In Data Vault 1.0, relationships between entities were defined using a combination of business keys and surrogate keys. Business keys are natural keys that identify an entity in the real world, while surrogate keys are system-generated keys used to uniquely identify an entity in the data warehouse. The combination of business keys and surrogate keys was used to link entities together, but this approach had some limitations.

Data Vault 2.0 introduced the concept of a Hash Key, which is a system-generated key that is based on the values of the attributes of an entity. The Hash Key is generated using a hash function, which takes the values of the attributes and converts them into a unique string of characters. The Hash Key is used to link entities together, replacing the combination of business keys and surrogate keys used in Data Vault 1.0. Here are some advantages of using a Hash Key in Data Vault 2.0:

1. Better scalability: Using a Hash Key allows for better scalability when dealing with large data volumes. Because the Hash Key is generated based on the values of the attributes, it is possible to use it to partition data across multiple nodes in a distributed environment.
2. Improved performance: Because the Hash Key is a single value, it is easier and faster to compare and search for entities. This can lead to improved query performance and faster data retrieval times.
3. Simplified modeling: Using a Hash Key simplifies the modeling process by removing the need to create and manage surrogate keys. This can make the modeling process faster and less error-prone.
4. Improved resilience: Using a Hash Key can improve the resilience of the data warehouse by reducing the likelihood of collisions between surrogate keys. Collisions can occur when two different entities have the same surrogate key, which can lead to data inconsistencies and errors.

In summary, using a Hash Key in Data Vault 2.0 provides several advantages over the absence of a Hash Key in Data Vault 1.0, including better scalability, improved performance, simplified modeling, and improved resilience.
