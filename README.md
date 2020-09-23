# Kafka-installation

## Software download
Download the software form Apache organization through the following link: [https://www.apache.org/dyn/closer.cgi?path=/kafka/2.6.0/kafka_2.13-2.6.0.tgz](https://www.apache.org/dyn/closer.cgi?path=/kafka/2.6.0/kafka_2.13-2.6.0.tgz)
## kafka services 
1. In order to start the zookeeper service, open powershell as Administrator in the kafka folder and run the following command <br/>
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
1. Now open another powershell as Administrator window and run the kafka service in  <br/>
.\bin\windows\kafka-server-start.bat .\config\server.properties
1. My topic is "iphone14-features"
1. Some features which I have listed are, "double tap on back","translate app"
1. To start the kafka producer, <br/>
.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic daily-routine <br/>
This is the producer where I have entered the iphone14-features
1. Starting kafka consumer, <br/>
.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic daily-routine --from-beginning <br/>
Here, we can view the different features entered
