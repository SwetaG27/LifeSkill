# Apache Kafka 
 
* It is a open source platform for stream-processing and distributed event stores.
 
 * It is commonly utilized for processing data in real-time.
 
 * Think about a newspaper delivery system, the producer is the printing press, the consumer is the reader, and Kafka is the delivery system ensuring newspapers reach on time.
  
      ![Apache_Kafka.md](/pictures/structure.png)
 

### Kafka Producer

   A Producer is an application or system that sends new data to Kafka.
 
 1. Think of the producer as the publisher of newspapers in our analogy.

 2. It sends data to specific topics within the Kafka cluster. For example:

     *  A weather app sending live temperature data to Kafka.
  
     *  An e-commerce website logging user activity for real-time analysis.
 
 ### Kafka Cluster

 A Kafka Cluster is a group of Kafka Brokers working together.

1. Each broker is a Kafka server that handles read and write requests from clients and stores data.
   
2. For fault tolerance and scalability, multiple brokers collaborate in a cluster. For example:
    * Imagine multiple warehouses working together to store and distribute products. These warehouses are your brokers, and the collective system is the Kafka cluster.
  
### Kafka Consumer
A Consumer is an application that reads data from Kafka. 

1. Consumers subscribe to specific topics and process the incoming data. For example:
   
   * A stock trading app might consume live market data to update prices on the user’s screen.

### Kafka Broker
A Broker is a single Kafka server.

1. Each broker has a unique ID and is responsible for storing specific portions of data.
   
2. Brokers distribute incoming data (messages) among themselves based on topics and partitions.

3. Even if one broker goes down, the cluster can recover using replicated data stored on other brokers.

### Kafka Partitions
Partitions break a topic into smaller parts for scalability and fault tolerance.

![Apache_Kafka.md](/pictures/partitions.png)

1. Each topic is divided into one or more partitions.
   * Example: Think of partitions as pages of a book within a topic.
   
2. Each page holds a portion of the topic's data.
   
3. **Benefits of partitions:**
   *  **Parallel processing:** Multiple consumers can read from partitions simultaneously.
   *   **Fault tolerance:** Data is replicated across partitions for recovery during failures.

### Kafka Connect
1. Kafka Connect allows you to integrate Kafka with other systems without writing code.

2. It’s used to move data in and out of Kafka, such as importing data from a database or exporting data to a data warehouse.
   * Example: If you want to sync data from your MySQL database into Kafka for real-time processing, Kafka Connect can handle this without requiring you to write complex scripts.
  
### Kafka Streams

1. Kafka Streams is a library for building stream processing applications.

2. It allows you to transform, aggregate, or filter data as it flows through Kafka. For example: 
   
     * Imagine you have a stream of purchase data. You can use Kafka Streams to calculate real-time sales trends, such as total revenue per minute.
 
 ## Apache Kafka Applications

 Nowdays demand for Apache Kafka is increasing at a tremendous speed. Many best enterprises today make use of Kafka to ease and grow their data pipelining requirements.

 ![Apache_kafka.md](/pictures/Application.png)


## Advantages of Apache Kafka

Following advantages of Apache Kafka makes it worthy:

1. **Low Latency:** Apache Kafka offers low latency value, i.e., upto 10 milliseconds. It is because it decouples the message which lets the consumer to consume that message anytime.
   
2. **High Throughput:** Due to low latency, Kafka is able to handle more number of messages of high volume and high velocity. Kafka can support thousands of messages in a second. Many companies such as Uber use Kafka to load a high volume of data.
   
3. **Fault tolerance:** Kafka has an essential feature to provide resistant to node/machine failure within the cluster.
   
4. **Durability:** Kafka offers the replication feature, which makes data or messages to persist more on the cluster over a disk. This makes it durable.
   
5. **Easily accessible:** As all our data gets stored in Kafka, it becomes easily accessible to anyone.

6. **Real-Time handling:** Apache Kafka is able to handle real-time data pipeline. Building a real-time data pipeline includes processors, analytics, storage, etc.
   
7. **Batch approach:** Kafka uses batch-like use cases. It can also work like an ETL tool because of its data persistence capability.
   
8. **Scalability:** The quality of Kafka to handle large amount of messages simultaneously make it a scalable software product.


## Disadvantages Of Apache Kafka


1. Do not have complete set of monitoring tools.
   
   
2. Do not support wildcard topic selection.

3. Brokers and consumers reduce the performance of Kafka by compressing and decompressing the data flow. 
   
4. It most often behaves a bit clumsy when the number of queues increases in the Kafka Cluster.
   
5. Certain message paradigms such as point-to-point queues, request/reply, etc. are missing in Kafka for some use cases.

## References 
 
* https://en.wikipedia.org/wiki/Apache_Kafka
 
* https://dev.to/renukapatil/mastering-apache-kafka-a-complete-guide-to-the-heart-of-real-time-data-streaming-3456
 
* https://www.projectpro.io/article/apache-kafka-architecture-/442

* https://www.javatpoint.com/apache-kafka-applications

* https://www.javatpoint.com/apache-kafka-advantages-and-disadvantages
 
  
 
 
