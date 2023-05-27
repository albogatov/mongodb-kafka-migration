First tasks done with:
- docker-compose.yaml
- sourceTopic and destinationTopic for Kafka Connectors

To start containers use ./start.sh

To read data on second MongoDB node use connection cmd: mongosh "mongodb://mongo2"

Data enter example: db.users.insertOne({ firstname: "abc", lastname: "bcd", age: 15, email: "bvb@gmail.com" })

Second task done with
- sourceTopic improved by adding a schema, no additional module was used

Data enter example for task two:
- db.users.insertOne({ firstname: "abc", lastname: "bcd", age: 15, email: "bvb@gmail.com", sex: "M" })

Third task done with:
- docker-compose.yaml

To start containers and initiate DB use ./start.sh
To see DB changes after posting data connect with: docker exec -it clickhouse-kafka-server-1 clickhouse-client