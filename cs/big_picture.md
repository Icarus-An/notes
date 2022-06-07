# Big Picture
- CICD pipeline
- Redis usage
- Java IoC >
- Java stack memory heap memory >
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

- Java data type
    - Primitive Data types
        - byte, short, int and long data types are used for storing whole numbers.
        - float and double are used for fractional numbers.
        - char is used for storing characters(letters).
        - boolean data type is used for variables that holds either true or false.

    - double type calculation will cause precision loss, occurred during conversing the decimal number into binary. Use BigDecimal with Stirng constructor to solve this problem.

    (1) 商业计算使用BigDecimal。
    (2) 使用参数类型为String的构造函数。
    (3) BigDecimal都是不可变的（immutable）的，在进行每一步运算时，都会产生一个新的对象，所以在做加减乘除运算时千万要保存操作后的值。

- Java 8 features.
    1. Java 8 – Lambda Expression
    2. Java 8 – Method references
    3. Java 8 – Functional interfaces
    4. Java 8 – Interface changes: Default and static methods
    5. Java 8 – Streams
    6. Java 8 – Stream filter
    7. Java 8 – forEach()
    8. Java 8 – Collectors class with example
    9. Java 8 – StringJoiner class with example
    10. Java 8 – Optional class with example
    11. Java 8 – Arrays Parallel Sort
