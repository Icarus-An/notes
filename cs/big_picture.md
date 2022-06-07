# Big Picture
- CICD pipeline
- Redis usage
- Java IoC
- Java stack memory heap memory
- state machine stock algorithm
- Triangle arbitrage algorithm
- spring boot

- Spring Security -JWT
- Agile - Scrum, CI

- kafka, ZooKeeper
    - Kafka: 4 major components (https://www.edureka.co/blog/interview-questions/top-apache-kafka-interview-questions-for-beginners/)
        - Topic: a stream of messages belonging to the same type
        - Producer: that can publish messages to a topic
        - Broker: a set of servers where the publishes messages are stored
        - Consumer: that subscribes to various topics and pulls data from the brokers.

    - ZooKeeper: CAP theroem (https://www.bmc.com/blogs/cap-theorem/)
        Consistency. All reads receive the most recent write or an error.
        Availability. All reads contain data, but it might not be the most recent.
        Partition tolerance. The system continues to operate despite network failures (ie; dropped partitions, slow network connections, or unavailable network connections between nodes.)
        Eureka in spring cloud ensured A&P, Zookeeper ensured C&P.

        Kafka uses Zookeeper to store offsets of messages consumed for a specific topic and partition by a specific Consumer Group.

- OOP
- Data base design
- multithread
