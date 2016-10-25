# iot-traffic-monitor-flink
Monitoring Traffic signal monitoring  using Apache Flink. 

This is a Apache flink implementation of ideas laid downhere (https://www.infoq.com/articles/traffic-data-monitoring-iot-kafka-and-spark-streaming).
This application will process real time IoT data sent by connected vehicles and use that data to monitor the traffic on different routes. 

###Pre-Requiste
1.Install Apache flink (https://ci.apache.org/projects/flink/flink-docs-release-1.2/quickstart/setup_quickstart.html)

2.Install Kafka and run a 2/3 broker for fault tolerance.(https://dtflaneur.wordpress.com/2015/10/05/installing-kafka-on-mac-osx/)

3.Creata a kfka topic using below command.
```javascript
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 3 --partitions 1 --topic iot-data-event-flink
```
###Overview



