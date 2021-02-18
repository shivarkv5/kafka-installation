# kafka-installation

## To download kafka

$ tar -xzf kafka_2.13-2.7.0.tgz
$ cd kafka_2.13-2.7.0


## To run ZooKeeper service

.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

## To run Kafka service

.\bin\windows\kafka-server-start.bat .\config\server.properties

## One time commands 

.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic alex-messages

.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list

## To run Kafka producer

.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic alex-messages

## To run kafka consumer.

.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic alex-messages --from-beginning
