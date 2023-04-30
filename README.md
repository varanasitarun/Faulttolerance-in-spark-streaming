This repo has coding sample program for different usecases

In this repository I have perfrmed checkpoiting and dynamic allocation in spark streaming. The main objective of checkpoiting feature is to recover failure messages and can be processed by the spark job. Here we have tested this scenario using the kafka producer. And also I have created test case for that.

Prior steps before running the code

1. Starting zookeeper server by using command zookeeper-server-start.bat ..\..\config\zookeeper.properties
2. Starting the kafka sever by using command  kafka-server-start.bat ..\..\config\server.properties
3. Create kafka topic by using command kafka-topics.bat --create --topic my-topic --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3
4. Start kafka-producer server by using command kafka-console-producer.bat --broker-list localhost:9092 --topic my-topic

We need to start all the servers by going to the directory where it is installed something like below

downloads/kafka/kafka/bin/windows

And then we can start the MyStructuredSparkStreaming.Java file by running the file. We have to download any IDE like eclipse,VSCode or intelliJ to run the code. Apart from that make sure to have the java installed and to the path correctly.

