# Ingesting MongoDB change events

This module defines the connector that ingests change events from MongoDB databases.

## Build

```
debezium build - mvn clean install -DskipITs -Denforcer.skip=true  -DskipTests
```
## Docker 

```
docker build -t data-platform/debezium-connector-mongodb:test .
docker tag data-platform/debezium-connector-mongodb:test 612427630422.dkr.ecr.us-east-1.amazonaws.com/data-platform/debezium-connector-mongodb:test
docker push 612427630422.dkr.ecr.us-east-1.amazonaws.com/data-platform/debezium-connector-mongodb:test
```

## GitHub Branch

There are two branched is being used
* `debezium-connector-mongodb/1.5.0-db` - MongoDB oplogs's db name will be used in Kafka topic name.
* `debezium-connector-mongodb/1.5.0-collection` - MongoDB oplogs's collection name will be used in Kafka topic name.

