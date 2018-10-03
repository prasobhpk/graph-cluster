# graph-cluster
Creating neo4j cluster using open source copy of neo4j enterprise : GraphStack Enterprise 

# How to start the neo4j cluster?

open terminal and run 
  ```
  docker-compose up

  ```
  
# Explore data and run queries using Neo4j Browser

The cluster instances are configured for HTTP access on ports 7474, 7475, 7476, 7477 and 7978. Just as you would on a standalone Neo4j, you can use these ports and a web browser to access the Neo4j Browser and explore data and run queries.

# Master vs Slave

Using a neo4j cluster is alomost like using a standalone Neo4j instance, except the write operations are only allowed through master(**Leader**).If you try to execute a write operation through a non-master instance, the write will be rejected and neo4j browser shows the error details.

# How to stop the neo4j cluster ?

open terminal and run 
  ```
  docker-compose down

  ```



For more deatils on cluster configuration refer : [neo4j clustering!](https://neo4j.com/docs/operations-manual/3.4/clustering/setup-new-cluster/)
