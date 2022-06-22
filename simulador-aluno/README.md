docker-compose up -d
docker exec -it kafka-kafka-1 bash
kafka-console-consumer --bootstrap-server=localhost:9092 --topic=readtest
kafka-console-producer --bootstrap-server=localhost:9092 --topic=readtest
kafka-console-consumer --bootstrap-server=localhost:9092 --topic=route.new-p
osition --group=terminal
kafka-console-producer --bootstrap-server=localhost:9092 --topic=route.new-direction