 #system-design 

## Computing
#cloud-computing

What is elastic computing?
?
Utilizes cloud services to automatically scale computing resources up or down based on workload, optimizing performance and cost efficiency.

What is serverless computing?
?
Enables developers to build and run applications without managing server infrastructure, automatically scaling based on demand.

What is hybrid cloud?
?
Combines on-premises infrastructure with cloud resources, providing flexibility and scalability based on specific workload demands.

Given an event-driven architectured application with serverless computing, what acceptable cloud solutions can be used to build the application to scale automatically based on demand?
?
AWS Lambda, Azure Functions.

Given a solution that needs to be deployed across multiple cloud providers for increased resilience, flexibility and scalability, what solutions could you implement?
?
Google Anthos, Red Hat OpenShift

Given an IoT platform with Edge Computing that distributes computing resources closer to IoT devices, allowing for scalable and efficient processing of data at the edge, what industry solutions could you implement this with?
?
Microsoft Azure IoT Edge, AWS IoT Greengrass
## Load balancing and scaling
#load-balancers #scalability 

What is load balancing?
?
Distributes incoming network traffic across multiple servers to ensure no single server is overwhelmed, improving both availability and responsiveness.

Given an e-commerce platform, how can one horizontally scale the solution?
?
By using balancing the load by using nginx-like software or by using cloud computing features such as Amazons EC2 Auto Scaling. You can deploy e-commerce applications on scalable cloud infrastructure, automatically adding or removing instances based on demand.

What is horizontal scaling?
?
Adds more instances of servers or nodes to a system to handle increased load, distributing the workload across multiple machines.

What is nginx and list some of its features? #load-balancers
?
- A widely used and effective load balancer. When implementing a load balancer, it's important to consider the specific requirements of your application, the anticipated traffic patterns, and the features provided by the load balancing solution. Nginx is just one example among several effective load balancers available in the market. Other options include HAProxy, Apache HTTP Server with mod_proxy, and cloud provider-specific load balancers.
- Effective and lightweight
- Load balancing algorithms
- Reverse proxy capabilities
- SSL termination #ssl
- Health checks
- WebSocket support
- Caching #caching
- Ease of configuration
- Active community and support
- Scalability #scalability
- Open Source
- Compatible with various protocols and application services
## Microservices
#microservices 

What are microservices?
?
Decomposes a monolithic application into smaller, independent services that can be developed, deployed, and scaled independently, enhancing flexibility and scalability.

Given a web application that needs to scale, what industry solution could be used?
?
Using Kubernetes for microservices containerization and orchestration.

## Caching
#caching 

What is caching? 
?
Stores frequently accessed data in memory to reduce the load on databases and improve response times.

Given a web application that loads static content like images and videos, what caching strategy can be used?
?
Use a Content Delivery Network (CDN) by distributing static content (images, videos, etc.) across globally distributed servers to reduce latency and improve content delivery times. Leverage solutions such as Amazon CloudFront, Akamai, Cloudflare.

What is a CDN?
?
Distributes content (such as images, videos, and web pages) across multiple servers located in various geographical locations, reducing latency and improving load times.

## Database
#databases 

What is a distributed database?
?
Distributes data across multiple servers or nodes, allowing for horizontal scaling and improved data retrieval and storage performance.

What is sharding?
?
Distributes a large database across multiple servers or clusters based on specific criteria, enabling horizontal scaling and improved data retrieval.

Given a social media platform where you would need to scale your database, what approach would you take and with what potential software or services?
?
Using  MongoDB sharding or Cassandra I could distribute user data across multiple database servers using sharding to handle the increasing volume of social media interactions.

## Big data
#databases 

Given an application that processed Big Data, what industry solution could be used to process and analyze large datasets in a distributed and scalable manner?
?
Using Hadoop's MapReduce paradigm or Apache Spark.

What is Big Data?
?
Big data refers to extremely large and complex datasets that are beyond the capacity of traditional data processing tools to capture, store, manage, and analyze within a reasonable time frame. Big data is characterised by a bunch of Vs:
- **Volume**: Big data involves a massive amount of information. This can range from terabytes to petabytes or even exabytes of data, generated from various sources such as social media, sensors, devices, and business transactions.
- **Velocity**: The speed at which data is generated, collected, and processed is a crucial aspect of big data. Streaming data, real-time analytics, and rapidly changing datasets contribute to the velocity of big data.
- **Variety**: Big data encompasses diverse types of data, including structured data (like databases and tables), unstructured data (such as text, images, and videos), and semi-structured data (like JSON or XML files). The variety of data types adds complexity to data processing and analysis.
- **Veracity**: Refers to the reliability and accuracy of the data. With big data, there can be challenges related to the quality and trustworthiness of the information.
- **Value**: The ultimate goal of big data is to derive meaningful insights and value from the vast amount of information collected. Extracting actionable insights can lead to better decision-making and improved business outcomes.

What technologies and tools can one use for big data and why is it valuable?
?
Big data technologies and analytics tools, such as Apache Hadoop, Apache Spark, and machine learning algorithms, are employed to process and analyze these large and complex datasets. The insights gained from big data analysis can be valuable for businesses, researchers, and organizations in various industries, enabling them to make data-driven decisions and gain a deeper understanding of patterns, trends, and correlations within the data.
## Networks

What is a peer-to-peer network?
?
Distributes tasks or content across multiple peer nodes, allowing for a decentralized architecture that can scale with the number of participating peers.

## Stateless

What is stateless architecture?
?
Designs applications where each request from a client is independent and doesn't rely on the state stored on the server, facilitating horizontal scaling.

## Immutable infrastructure

What is immutable infrastructure?
?
Treats infrastructure as code and replaces existing instances rather than modifying them, allowing for easy and efficient scaling.

## Parallel

What is parallel processing?
?
Divides a task into subtasks that can be processed simultaneously, leveraging parallel computing to improve performance and scalability.

## Event-driven architecture

![[Introduction to Event-Driven Architecture.png]]

What is event-driven architecture?
?
Utilizes events to trigger and communicate between different components, allowing for a scalable and loosely coupled system.

Given an application, what could you use to implement scalable stream processing for real-time data analytics and event-driven applications?
? 
Apache Flink.

What is asynchronous messaging?
?
Uses message queues or publish-subscribe patterns to decouple components, allowing for better scalability and fault tolerance.

Given an application with real-time analytics, what could you potentially use to implement a scalable, distributed event streaming platform for real-time analytics and data processing?
?
Apache Kafka

Given a Fintech application, what practical approach could you develop the solution in for scalability and resilience?
?
Using CQRS and Event Sourcing with Apache Kafka, Axon Framework

What is CQRS?
?
CQRS, or Command Query Responsibility Segregation, is a software architectural pattern that suggests separating the concerns of handling command (write) operations from query (read) operations in a system. Instead of using a single model to perform both read and write operations, CQRS advocates having separate models optimized for each type of operation. This pattern helps in designing more scalable and efficient systems, especially in scenarios where read and write requirements differ significantly

What are the key principles of CQRS?
?
1. **Separation of Concerns:**
    CQRS encourages dividing the application logic into distinct components for handling commands and queries, minimizing the complexity of a single model.
2. **Different Models for Reads and Writes:**
	Designing separate models for read and write operations allows each model to be optimized for its specific use case. Write models can be more focused on enforcing business rules, while read models can be tailored for efficient querying and presentation.
1. **Asynchronous Communication:**
    CQRS often involves using asynchronous communication between the command and query components. This can be implemented through event sourcing, message queues, or other communication mechanisms.
4. **Scalability:**
    The separation of read and write models facilitates better scalability. For example, read models can be replicated, cached, or denormalized to optimize query performance without impacting the consistency requirements of the write models.
5. **Flexibility and Maintainability:**
    CQRS can make systems more flexible and maintainable by allowing changes to one part of the system without affecting the other. This separation also enables the use of different technologies and storage mechanisms for read and write models.
6. **Event Sourcing:**
    Often used in conjunction with CQRS, event sourcing involves capturing all changes to the application state as a sequence of events. These events can be used to build and rebuild the application state, providing a historical record of changes.

What is the trade off of using CQRS?
?
It's important to note that while CQRS can provide benefits in terms of scalability and separation of concerns, it may introduce additional complexity to the system. It is typically applied in scenarios where the advantages of separate models for reads and writes outweigh the complexities introduced by the pattern. CQRS is commonly used in conjunction with event sourcing and is often associated with Domain-Driven Design (DDD).

## Federated architecture

What is federated architecture?
?
Connects multiple autonomous systems or services, enabling scalability and collaboration across different entities.