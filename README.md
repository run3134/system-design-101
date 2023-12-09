<p>
  <a href="https://blog.bytebytego.com/?utm_source=site"><img src="images/banner.jpg" /> </a>
</p>

<p align="center">
  【
  <a href="https://www.youtube.com/channel/UCZgt6AzoyjslHTC9dz0UoTw">
    👨🏻‍💻 YouTube
  </a> | 
  <a href="https://blog.bytebytego.com/?utm_source=site">
    📮 Newsletter
  </a> 】
</p>

<a href="https://trendshift.io/repositories/3709" target="_blank"><img src="https://trendshift.io/api/badge/repositories/3709" alt="ByteByteGoHq%2Fsystem-design-101 | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

# System Design 101

Explain complex systems using visuals and simple terms. 

Whether you're preparing for a System Design Interview or you simply want to understand how systems work beneath the surface, we hope this repository will help you achieve that.

# Table of Contents

<!-- TOC toc.levels=2 -->
- [Architecture patterns](#architecture-patterns)
  - [MVC, MVP, MVVM, MVVM-C, and VIPER](#mvc-mvp-mvvm-mvvm-c-and-viper)
  - [18 Key Design Patterns Every Developer Should Know](#18-key-design-patterns-every-developer-should-know)
- [Microservice architecture](#microservice-architecture)
  - [What does a typical microservice architecture look like?](#what-does-a-typical-microservice-architecture-look-like)
  - [Microservice Best Practices](#microservice-best-practices)
  - [What tech stack is commonly used for microservices?](#what-tech-stack-is-commonly-used-for-microservices)
  - [Why is Kafka fast](#why-is-kafka-fast)  
- [Communication protocols](#communication-protocols)
  - [REST API vs. GraphQL](#rest-api-vs-graphql)
  - [How does gRPC work?](#how-does-grpc-work)
  - [What is a webhook?](#what-is-a-webhook)
  - [How to improve API performance?](#how-to-improve-api-performance)
  - [HTTP 1.0 -\> HTTP 1.1 -\> HTTP 2.0 -\> HTTP 3.0 (QUIC)](#http-10---http-11---http-20---http-30-quic)
  - [SOAP vs REST vs GraphQL vs RPC](#soap-vs-rest-vs-graphql-vs-rpc)
  - [Code First vs. API First](#code-first-vs-api-first)
  - [HTTP status codes](#http-status-codes)
  - [What does API gateway do?](#what-does-api-gateway-do)
  - [How do we design effective and safe APIs?](#how-do-we-design-effective-and-safe-apis)
  - [TCP/IP encapsulation](#tcpip-encapsulation)
  - [Why is Nginx called a “reverse” proxy?](#why-is-nginx-called-a-reverse-proxy)
  - [What are the common load-balancing algorithms?](#what-are-the-common-load-balancing-algorithms)
  - [URL, URI, URN - Do you know the differences?](#url-uri-urn---do-you-know-the-differences)
- [Database](#database)
  - [A nice cheat sheet of different databases in cloud services](#a-nice-cheat-sheet-of-different-databases-in-cloud-services)
  - [8 Data Structures That Power Your Databases](#8-data-structures-that-power-your-databases)
  - [How is an SQL statement executed in the database?](#how-is-an-sql-statement-executed-in-the-database)
  - [CAP theorem](#cap-theorem)
  - [Types of Memory and Storage](#types-of-memory-and-storage)
  - [Visualizing a SQL query](#visualizing-a-sql-query)
  - [SQL language](#sql-language)
- [Cache](#cache)
  - [Data is cached everywhere](#data-is-cached-everywhere)
  - [Why is Redis so fast?](#why-is-redis-so-fast)
  - [How can Redis be used?](#how-can-redis-be-used)
  - [Top caching strategies](#top-caching-strategies)
- [Payment systems](#payment-systems)
  - [How to learn payment systems?](#how-to-learn-payment-systems)
  - [Why is the credit card called “the most profitable product in banks”? How does VISA/Mastercard make money?](#why-is-the-credit-card-called-the-most-profitable-product-in-banks-how-does-visamastercard-make-money)
  - [How does VISA work when we swipe a credit card at a merchant’s shop?](#how-does-visa-work-when-we-swipe-a-credit-card-at-a-merchants-shop)
  - [Payment Systems Around The World Series (Part 1): Unified Payments Interface (UPI) in India](#payment-systems-around-the-world-series-part-1-unified-payments-interface-upi-in-india)
- [CI/CD](#cicd)
  - [CI/CD Pipeline Explained in Simple Terms](#cicd-pipeline-explained-in-simple-terms)
  - [Netflix Tech Stack (CI/CD Pipeline)](#netflix-tech-stack-cicd-pipeline)
- [DevOps](#devops)
  - [DevOps vs. SRE vs. Platform Engineering. What is the difference?](#devops-vs-sre-vs-platform-engineering-what-is-the-difference)
  - [What is k8s (Kubernetes)?](#what-is-k8s-kubernetes)
  - [Docker vs. Kubernetes. Which one should we use?](#docker-vs-kubernetes-which-one-should-we-use)
  - [How does Docker work?](#how-does-docker-work)
- [GIT](#git)
  - [How Git Commands work](#how-git-commands-work)
  - [How does Git Work?](#how-does-git-work)
  - [Git merge vs. Git rebase](#git-merge-vs-git-rebase)
- [Cloud Services](#cloud-services)
  - [A nice cheat sheet of different cloud services (2023 edition)](#a-nice-cheat-sheet-of-different-cloud-services-2023-edition)
  - [What is cloud native?](#what-is-cloud-native)
- [Developer productivity tools](#developer-productivity-tools)
  - [Visualize JSON files](#visualize-json-files)
  - [Automatically turn code into architecture diagrams](#automatically-turn-code-into-architecture-diagrams)
- [Linux](#linux)
  - [Linux file system explained](#linux-file-system-explained)
  - [18 Most-used Linux Commands You Should Know](#18-most-used-linux-commands-you-should-know)
- [Security](#security)
  - [How does HTTPS work?](#how-does-https-work)
  - [Oauth 2.0 Explained With Simple Terms.](#oauth-20-explained-with-simple-terms)
  - [Top 4 Forms of Authentication Mechanisms](#top-4-forms-of-authentication-mechanisms)
  - [Session, cookie, JWT, token, SSO, and OAuth 2.0 - what are they?](#session-cookie-jwt-token-sso-and-oauth-20---what-are-they)
  - [How to store passwords safely in the database and how to validate a password?](#how-to-store-passwords-safely-in-the-database-and-how-to-validate-a-password)
  - [Explaining JSON Web Token (JWT) to a 10 year old Kid](#explaining-json-web-token-jwt-to-a-10-year-old-kid)
  - [How does Google Authenticator (or other types of 2-factor authenticators) work?](#how-does-google-authenticator-or-other-types-of-2-factor-authenticators-work)
- [Real World Case Studies](#real-world-case-studies)
  - [Netflix's Tech Stack](#netflixs-tech-stack)
  - [Twitter Architecture 2022](#twitter-architecture-2022)
  - [Evolution of Airbnb’s microservice architecture over the past 15 years](#evolution-of-airbnbs-microservice-architecture-over-the-past-15-years)
  - [Monorepo vs. Microrepo.](#monorepo-vs-microrepo)
  - [How will you design the Stack Overflow website?](#how-will-you-design-the-stack-overflow-website)
  - [Why did Amazon Prime Video monitoring move from serverless to monolithic? How can it save 90% cost?](#why-did-amazon-prime-video-monitoring-move-from-serverless-to-monolithic-how-can-it-save-90-cost)
  - [How does Disney Hotstar capture 5 Billion Emojis during a tournament?](#how-does-disney-hotstar-capture-5-billion-emojis-during-a-tournament)
  - [How Discord Stores Trillions Of Messages](#how-discord-stores-trillions-of-messages)
  - [How do video live streamings work on YouTube, TikTok live, or Twitch?](#how-do-video-live-streamings-work-on-youtube-tiktok-live-or-twitch)

<!-- /TOC -->

## Architecture patterns

### MVC, MVP, MVVM, MVVM-C, and VIPER
These architecture patterns are among the most commonly used in app development, whether on iOS or Android platforms. Developers have introduced them to overcome the limitations of earlier patterns. So, how do they differ? 

<p>
  <img src="images/client arch patterns.png" style="width: 720px" />
</p>

* MVC, the oldest pattern, dates back almost 50 years 
  - https://github.com/run3134/system-design-101/blob/main/README.md#architecture-patterns
  - Moel
    - has DB component
    - talk to DB, by get/set
    - it will be called by activities
  - View and Contoller are handled by activity
    - it listen to activities
    - when activity happens, it contains the logic how activity will be handled, how data in the model will be called
* Every pattern has a "view" (V) responsible for displaying content and receiving user input 
* Most patterns include a "model" (M) to manage business data 
* "Controller," "presenter," and "view-model" are translators that mediate between the view and the model ("entity" in the VIPER pattern)

### 18 Key Design Patterns Every Developer Should Know

Patterns are reusable templates to common design problems, 
- serving as blueprints for building better software structures. 
- resulting in a smoother, more efficient development process.
These are some of the most popular patterns: 

<p>
  <img src="images/18-oo-patterns.png" />
</p>

* creational pattern: These design patterns provide a way to create objects while hiding the creation logic, rather than instantiating objects directly using new operator. This gives program more flexibility in deciding which objects need to be created for a given use case.
  - Abstract Factory: Family Creator - Makes groups of related items. 
    - step1: create abstract class/interface
    - step2: define concrete class by implementing the interface
    - step3: create factory with method getShape(param)
    - step4: demo main
  - Builder: Lego Master - Builds objects step by step, keeping creation and appearance separate. 
    - step1: create simple object
    - step2: create complext object
  - Prototype: Clone Maker - Creates copies of fully prepared examples. (https://www.tutorialspoint.com/design_pattern/prototype_pattern.htm)
    - when it is costly to create from obj from scratch b/c of db call
    - step1: concrete class, with clone abilty
    - step2: cache of objects
    - step3: when need to create objects, check cache first; if in cache, then fetch+clone; otherwise, create+cache
  - Singleton: One and Only - A special class with just one instance. **when import the class: there is an unique instance**
    - step1: create class with private constructor
    - step2: initiate an instance of the class within the class definition
    - step3: provide method to fetch the instance
* structural pattern: These design patterns concern class and object composition. Concept of inheritance is used to compose interfaces and define ways to compose objects to obtain new functionalities.
  - Adapter: Universal Plug - Connects things with different interfaces. https://www.tutorialspoint.com/design_pattern/adapter_pattern.htm
    - step1: there are two interface, without any relationship
    - step2: adapter implement one interface(higher level), inside it has field which is type of detail interface
    - step3: when define the hgih level methods, it use parameterization
    - step4: then concrete class can implement high level class
  - Bridge: Function Connector - Links how an object works to what it does. 
    - create 一个instance 的时候，需要有param + 其他的instance
    - 其他instance 的class 可以evolve indpendently
  - Composite: Tree Builder - Forms tree-like structures of simple and complex parts. 
    - a class that contains group of its own objects
  - Decorator: Customizer - **Adds features** to objects without changing their core. 
    - step1: the original class is a field
    - step2: override the method with 
      - call the method by field.original_method()
      - add new functionality
  - Facade: One-Stop-Shop - Represents a whole system with a single, simplified interface. 
    - like combination of: factory + composition
    - when a facade is created: many instance are actualy created
    - we can have access to all functions by each instance or in parameterized way
  - Flyweight: Space Saver - Shares small, reusable items efficiently. 
    - like prototype to cache created obj
    - it also need to reset filed value, as we are not going to create new instance; reuse same instance by reset field values
  - Proxy: Stand-In Actor - Represents another object, controlling access or actions. 
    - the example: https://www.tutorialspoint.com/design_pattern/proxy_pattern.htm
    - it create lazy construction: actual instance is created until it is used
* behavioral pattern: These design patterns are specifically concerned with communication between objects.
  - Chain of Responsibility: Request Relay - Passes a request through a chain of objects until handled. 
    - normally each receiver contains reference to another receiver. If one object cannot handle the request then it passes the same to the next receiver and so on.
      - reference is set in field called: nextlogger
  - Command: Task Wrapper - Turns a request into an object, ready for action. 
    - 
  - Iterator: Collection Explorer - Accesses elements in a collection one by one. 
    - get a way to access the elements of a collection object in sequential manner without any need to know its underlying representation
  - Mediator: Communication Hub - Simplifies interactions between different classes. 
    - example: class chatRoom{ def showMsg(senderName, msg)}
    - each user has method:= send_msg, chatRoom, need to take that msg
    - **relationship between {users} and chatRoom???**
  - Memento: Time Capsule - Captures and restores an object's state. 
    - memento: one class state 
    - memos: queue of historical states
    - relationship between memos and oringinator
  - Observer: News Broadcaster - Notifies classes about changes in other objects. 
  - Visitor: Skillful Guest - Adds new operations to a class without altering it.


## Microservice architecture

### What does a typical microservice architecture look like? 

The diagram below shows a typical microservice architecture. 

<p>
  <img src="images/typical-microservice-arch.jpg" style="width: 520px" />
</p>


- Load Balancer: This distributes incoming traffic across multiple backend services. 
- CDN (Content Delivery Network): CDN is a group of geographically distributed servers that hold static content for faster delivery. The clients look for content in CDN first, then progress  to backend services.
- API Gateway: This handles incoming requests and routes them to the relevant services. It talks to the identity provider and service discovery.
- Identity Provider: This handles authentication and authorization for users. 
- Service Registry & Discovery: Microservice registration and discovery happen in this component, and the API gateway looks for relevant services in this component to talk to. 
- Management: This component is responsible for monitoring the services.
- Microservices: Microservices are designed and deployed in different domains. Each domain has its own database. The API gateway talks to the microservices via REST API or other protocols, and the microservices within the same domain talk to each other using RPC (Remote Procedure Call).

Benefits of microservices:
* decoupled
  - Each domain can be independently maintained by a dedicated team.
  - Business requirements can be customized in each domain and better supported, as a result.
  - They can be quickly designed, deployed, and horizontally scaled.


### What tech stack is commonly used for microservices?

Below you will find a diagram showing the microservice tech stack, both for the development phase and for production.

<p>
  <img src="images/microservice-tech.jpeg" />
</p>


▶️ 𝐏𝐫𝐞-𝐏𝐫𝐨𝐝𝐮𝐜𝐭𝐢𝐨𝐧

- Define API - This establishes a contract between frontend and backend. We can use Postman or OpenAPI for this.
- Development 
  - Node.js or react is popular for frontend development, 
  - and java/python/go for backend development. Also, we need to change the configurations in the API gateway according to API definitions.
- Continuous Integration - JUnit and Jenkins for automated testing. The code is packaged into a Docker image and deployed as microservices.

▶️ 𝐏𝐫𝐨𝐝𝐮𝐜𝐭𝐢𝐨𝐧 (map to a typical microservice architecture)

- load balancer: NGinx is a common choice for load balancers. 
- CDN: Cloudflare provides CDN (Content Delivery Network). 
- API Gateway: - We can use 
  - criteria
    - scale: how easy to scale; how much vol
    - latency
    - integration with graphQL, etc
  - spring boot for the gateway (https://www.solo.io/topics/api-gateway/api-gateway-spring-boot/)
    - how to use sprint cloud gateway: https://spring.io/guides/gs/gateway/
  - flask(https://www.reddit.com/r/flask/comments/etajkg/how_to_make_an_api_gateway_in_flask/)
    - authentication: https://www.digitalocean.com/community/tutorials/how-to-add-authentication-to-your-app-with-flask-login with flask-login library to handle user sessions
    - authorization: https://flask-authorize.readthedocs.io/en/latest/ from flask_authorize import Authorize
    - rate limit: https://medium.com/analytics-vidhya/how-to-rate-limit-routes-in-flask-61c6c791961b
- Service register/discovery: Eureka/Zookeeper for service discovery.
   - Eureka: https://spring.io/guides/gs/service-registration-and-discovery/
   - zookeeper: https://dzone.com/articles/zookeeper-for-microservice-registration-and-discov
- The microservices are deployed on clouds. We have options among AWS, Microsoft Azure, or Google GCP.
- Cache and Full-text Search - Redis is a common choice for caching key-value pairs. Elasticsearch is used for full-text search.
- Communications - For services to talk to each other, we can use messaging infra Kafka or RPC (https://www.quora.com/How-should-I-choose-between-gRPC-and-Kafka-when-building-microservices)
  - kafka push info to other services
    - async
    - it needs message broker to handle message delivery (at most once, at least once, exact once)
    - introducing something like Kafka adds to the overall complexity of your system, so you need to judge whether the benefits outweigh the costs of that
    - use case: 
      - data flow: take a stream of msg|events, transform it, and pass them to other services
  - rpc pull informace
    - sync
- Persistence - We can use MySQL or PostgreSQL for a relational database, and Amazon S3 for object store. We can also use Cassandra for the wide-column store if necessary.
- Management & Monitoring - To manage so many microservices, the common Ops tools include Prometheus, Elastic Stack, and Kubernetes.


### Microservice Best Practices

A picture is worth a thousand words: 9 best practices for developing microservices.

<p>
  <img src="images/microservice-best-practices.jpeg" />
</p>

 
When we develop microservices, we need to follow the following best practices: 
* design
  - Assign each microservice with a single responsibility 
  - Design stateless services 
  - Adopt domain-driven design
  - Design micro frontend 
  - Orchestrating microservices 
* code/dev
  - Keep code at a similar level of maturity 
  - Separate build for each microservice 
  - Deploy into containers 
  - Use separate data storage for each microservice 


### Why is Kafka fast

There are many design decisions that contributed to Kafka’s performance. In this post, we’ll focus on two. We think these two carried the most weight.

why Kafka is fast is? https://technology.inmobi.com/articles/2023/05/29/the-underlying-reason-behind-kafkas-speed
* its sequential I/O, stores all the data it ingests in a log-structured format, which means that new data is appended to the end of the log. This allows for very fast writes, since only the latest data needs to be appended, but it also means that older data needs to be periodically compacted to reclaim disk space.
  - disk
    - 316 values/sec
    - 53.2M values/sec
  - SSD
    - 2k
    - 42.2 M 
  - RAM
    - 36.7M
    - 358M
* zero copy principle (no temporary buffer): a traditional approach would be to copy the data from the source location to a temporary buffer, and then copy it again to the destination location. However, the zero-copy principle eliminates this intermediate step by allowing the data to be transferred directly from the source location to the destination location, without the need for an intermediate copy. 
  - memory mapping: a process to access a file or other data source as if it were in its own memory space
  - Direct memory access (DMA) device to directly access memory: This technique allows a device, such as a network card or disk controller, to transfer data directly to or from memory, without the need for the CPU to be involved in the transfer.
  - user space library: like zero-copy libraries can help to implement zero-copy principles and eliminate the unnecessary data copies.
  - traditional way: disk == read by os==> page cache in kernel -- read by app --> user space buffer 
    -- write by app --> socket buffer in kernel == copy by os ==> NIC
  - new way: by using sendfile system call, modern Unix operating systems like Linux can transfer data from page cache to a socket efficiently, avoiding unnecessary copies and system calls 
  - <p><img src="images/Kafka_sendfile.png" /></p>


<p>
  <img src="images/why_is_kafka_fast.jpeg" />
</p>


1. The first one is Kafka’s reliance on Sequential I/O.
2. The second design choice that gives Kafka its performance advantage is its focus on efficiency: zero copy principle.
 
The diagram illustrates how the data is transmitted between producer and consumer, and what zero-copy means.
 
- Step 1.1 - 1.3: Producer writes data to the disk 
- Step 2: Consumer reads data without zero-copy

2.1 The data is loaded from disk to OS cache

2.2 The data is copied from OS cache to Kafka application

2.3 Kafka application copies the data into the socket buffer 

2.4 The data is copied from socket buffer to network card

2.5 The network card sends data out to the consumer

 
- Step 3: Consumer reads data with zero-copy

3.1: The data is loaded from disk to OS cache
3.2 OS cache directly copies the data to the network card via sendfile() command
3.3 The network card sends data out to the consumer
 
Zero copy is a shortcut to save the multiple data copies between application context and kernel context.


## Communication protocols

Architecture styles define how different components of an application programming interface (API) interact with one another. As a result, they ensure efficiency, reliability, and ease of integration with other systems by providing a standard approach to designing and building APIs. Here are the most used styles:

<p>
  <img src="images/api-architecture-styles.png" style="width: 640px">
</p>

- SOAP: 

  Mature, comprehensive, XML-based
  
  Best for enterprise applications 

- RESTful: 

  Popular, easy-to-implement, HTTP methods 

  Ideal for web services 

- GraphQL: 

  Query language, request specific data 

  Reduces network overhead, faster responses 

- gRPC: 

  Modern, high-performance, Protocol Buffers 

  Suitable for microservices architectures 

- WebSocket: 

  Real-time, bidirectional, persistent connections 

  Perfect for low-latency data exchange 

- Webhook: 

  Event-driven, HTTP callbacks, asynchronous 

  Notifies systems when events occur


### REST API vs. GraphQL

When it comes to API design, REST and GraphQL each have their own strengths and weaknesses.

The diagram below shows a quick comparison between REST and GraphQL.

<p>
  <img src="images/graphQL.jpg">
</p>

https://aws.amazon.com/compare/the-difference-between-graphql-and-rest/
* in common
  - arch point of view
    - does not save response history between requests
    - client-server model, so requests from a single client result in replies from a single server
    - HTTP as underlying communication protocal
  - resource based design
    - each object in resources has unique id
    - 
  - data exchange
    - response in json format 
    - support caching
* difference
  - REST limitation
    - fixed-structure data exchange 
    - over fetching or under fetching
      - return data from same db
      - multiple query to retrieve data from multiple db
  - how to use
    - REST
      - HTTP verb : action; URL: resrouce to take action; param/value; example: GET /posts  # return all posts
    - GraphQL
      - query/mutation/subscription: example: GET /graphql?query{post(id: 1) {id title content}} #returns only the first post:
  
  - data access: REST has multiple endpoint, vs. graphQL only has one
  - data returned: REST server defined; graphQL client defined
  - use case: REST simple data structure, graphQL complex data structure
  - data type: REST weakly typed, graphQL strong typed

REST

- Uses standard HTTP methods like GET, POST, PUT, DELETE for CRUD operations.
- Works well when you need simple, uniform interfaces between separate services/applications.
- Caching strategies are straightforward to implement.
- The downside is it may require multiple roundtrips to assemble related data from separate endpoints.

GraphQL

- Provides a single endpoint for clients to query for precisely the data they need.
- Clients specify the exact fields required in nested queries, and the server returns optimized payloads containing just those fields.
- Supports Mutations for modifying data and Subscriptions for real-time notifications.
- Great for aggregating data from multiple sources and works well with rapidly evolving frontend requirements.
- However, it shifts complexity to the client side and can allow abusive queries if not properly safeguarded
- Caching strategies can be more complicated than REST.

The best choice between REST and GraphQL depends on the specific requirements of the application and development team. GraphQL is a good fit for complex or frequently changing frontend needs, while REST suits applications where simple and consistent contracts are preferred.

Neither API approach is a silver bullet. Carefully evaluating requirements and tradeoffs is important to pick the right style. Both REST and GraphQL are valid options for exposing data and powering modern applications.


### How does gRPC work?

RPC (Remote Procedure Call) is called “**remote**” because it enables communications between remote services when services are deployed to different servers under microservice architecture. From the user’s point of view, it acts like a local function call.

The diagram below illustrates the overall data flow for **gRPC**.

<p>
  <img src="images/grpc.jpg">
</p>

Step 1: A REST call is made from the client. The request body is usually in JSON format.

Steps 2 - 4: The order service (gRPC client) receives the REST call, transforms it, and makes an RPC call to the payment service. gRPC encodes the **client stub** into a binary format and sends it to the low-level transport layer.

Step 5: gRPC sends the packets over the network via HTTP2. Because of binary encoding and network optimizations, gRPC is said to be 5X faster than JSON.

Steps 6 - 8: The payment service (gRPC server) receives the packets from the network, decodes them, and invokes the server application.

Steps 9 - 11: The result is returned from the server application, and gets encoded and sent to the transport layer.

Steps 12 - 14: The order service receives the packets, decodes them, and sends the result to the client application.

是不是
* client side application often use rest or graphQL? 
* and internal service use gRPC calls
  - micro-service which provide the service, has proto/package defined
  - server side
    - define class, method
  - the client side just import the library and call the method
    - need to know how to connect to server, 
      - in python grpc.insecure_channel(target), secure_channel(target, CREDENTIAL)
      - the same for java
    - define service interface: several method, like , getXXXresponse(), getYYYresponse()
    - define rpcClient which implement service


### What is a webhook?

The diagram below shows a comparison between polling and Webhook. 

<p>
  <img src="images/webhook.jpeg" style="width: 680px" />
</p>

Assume we run an eCommerce website. The clients send orders to the order service via the API gateway, which goes to the payment service for payment transactions. The payment service then talks to an external payment service provider (PSP) to complete the transactions. 

There are two ways to handle communications with the external PSP. 

**1. Short polling** 

After sending the payment request to the PSP, the payment service keeps asking the PSP about the payment status. After several rounds, the PSP finally returns with the status. 

Short polling has two drawbacks: 
* Constant polling of the status requires resources from the payment service. 
* The External service communicates directly with the payment service, creating security vulnerabilities. 

**2. Webhook** 

We can register a webhook with the external service. It means: call me back at a certain URL when you have updates on the request. When the PSP has completed the processing, it will invoke the HTTP request to update the payment status.

In this way, the programming paradigm is changed, and the payment service doesn’t need to waste resources to poll the payment status anymore.

What if the PSP never calls back? We can set up a housekeeping job to check payment status every hour.

Webhooks are often referred to as reverse APIs or push APIs because the server sends HTTP requests to the client. We need to pay attention to 3 things when using a webhook:

1. We need to design a proper API for the external service to call.
2. We need to set up proper rules in the API gateway for security reasons.
3. We need to register the correct URL at the external service.

### How to improve API performance?

The diagram below shows 5 common tricks to improve API performance.

<p>
  <img src="images/api-performance.jpg">
</p>

1. client side, 
  - pagenation; if data is large, could be send by min batch, so client could start consume the data while other part of data is still on the way
2. server side: 
  - caching on server side to improve the responsiveness
  - async logging
3. internet connection: 
  - connection pool
  - payload compression: to improve the data transmit

Pagination

This is a common optimization when the size of the result is large. The results are streaming back to the client to improve the service responsiveness.

Asynchronous Logging

Synchronous logging deals with the disk for every call and can slow down the system. Asynchronous logging sends logs to a lock-free buffer first and immediately returns. The logs will be flushed to the disk periodically. This significantly reduces the I/O overhead.

Caching

We can cache frequently accessed data into a cache. The client can query the cache first instead of visiting the database directly. If there is a cache miss, the client can query from the database. Caches like Redis store data in memory, so the data access is much faster than the database.

Payload Compression

The requests and responses can be compressed using gzip etc so that the transmitted data size is much smaller. This speeds up the upload and download.

Connection Pool

When accessing resources, we often need to load data from the database. Opening the closing db connections adds significant overhead. So we should connect to the db via a pool of open connections. The connection pool is responsible for managing the connection lifecycle.

### HTTP 1.0 -> HTTP 1.1 -> HTTP 2.0 -> HTTP 3.0 (QUIC)

What problem does each generation of HTTP solve?

The diagram below illustrates the key features.

<p>
  <img src="images/http3.jpg" />
</p>

**HOL blocking** - A browser is total number of parallel requests, when it is used up, subsequent requests need to wait for the former ones to complete. 

- HTTP 1.0 was finalized and fully documented in 1996. Every request to the same server requires a separate TCP connection.

- HTTP 1.1 was published in 1997. A TCP connection can be left open for reuse (persistent connection), but it doesn’t solve the HOL (head-of-line) blocking issue. 

- HTTP 2.0 was published in 2015. It addresses HOL issue through request multiplexing, which eliminates HOL blocking at the application layer, but HOL still exists at the transport (TCP) layer.

  As you can see in the diagram, HTTP 2.0 introduced the concept of HTTP “streams”: an abstraction that "allows multiplexing different HTTP exchanges onto the same TCP connection". Each stream doesn’t need to be sent in order.

- HTTP 3.0 first draft was published in 2020. It is the proposed successor to HTTP 2.0. It uses QUIC instead of TCP for the underlying transport protocol, thus removing HOL blocking in the transport layer. 

QUIC is based on UDP. It introduces streams as first-class citizens at the transport layer. QUIC streams share the same QUIC connection, so no additional handshakes and slow starts are required to create new ones, but QUIC streams are delivered independently such that in most cases packet loss affecting one stream doesn't affect others.

### SOAP vs REST vs GraphQL vs RPC

The diagram below illustrates the API timeline and API styles comparison.

Over time, different API architectural styles are released. Each of them has its own patterns of standardizing data exchange. 

You can check out the use cases of each style in the diagram.

<p>
  <img src="images/SOAP vs REST vs GraphQL vs RPC.jpeg" />
</p>
**Why protocal matters?**
* HTTP is a TCP/IP based protocol. So when you use REST you are already using TCP for communication. But if you want to use REST over pure TCP socket, without HTTP, then no, this doesn't make sense because REST is based on HTTP verbs and headers. Those notions exist only in the HTTP protocol. REST -> HTTP -> TCP
* RPC uses HTTP/2 under the covers, but HTTP is not exposed to the API designer. gRPC-generated stubs and skeletons hide HTTP from the client and server too, so nobody has to worry how the RPC concepts are mapped to HTTP—they just have to learn gRPC. 


### Code First vs. API First 

The diagram below shows the differences between code-first development and API-first development. Why do we want to consider API first design?

<p>
  <img src="images/api_first.jpg" style="width: 680px" />
</p>
1. API first <=> microservice
2. microservice: decoupling/segregation of big duty
3. collaboration via same language: API, less surprise
4. system test could be easier, just mock request/response

- Microservices increase system complexity and we have separate services to serve different functions of the system. While this kind of architecture facilitates decoupling and segregation of duty, we need to handle the various communications among services. 

It is better to think through the system's complexity before writing the code and carefully defining the boundaries of the services.

- Separate functional teams need to speak the same language and the dedicated functional teams are only responsible for their own components and services. It is recommended that the organization speak the same language via API design. 

We can mock requests and responses to validate the API design before writing code.

- Improve software quality and developer productivity Since we have ironed out most of the uncertainties when the project starts, the overall development process is smoother, and the software quality is greatly improved. 

Developers are happy about the process as well because they can focus on functional development instead of negotiating sudden changes.

The possibility of having surprises toward the end of the project lifecycle is reduced.

Because we have designed the API first, the tests can be designed while the code is being developed. In a way, we also have TDD (Test Driven Design) when using API first development.

### HTTP status codes

<p>
  <img src="images/http-status-code.jpg" style="width: 540px" />
</p>


The response codes for HTTP are divided into five categories: 

Informational (100-199) 
Success (200-299) 
Redirection (300-399) 
Client Error (400-499) 
Server Error (500-599) 

### What does API gateway do? 

The diagram below shows the details. 

<p>
  <img src="images/api_gateway.jpg" style="width: 520px" />
</p>

API gateway responsibility
* parse info/attributes from http request
  - check user id based allow/deny list
  - ID: authentication password
  - rate limit 
* route the request to proper backend microservice 
* improvement
  - caching
* misc functions
  - error handling 
  - logging
  - monitoring

Step 1 - The client sends an HTTP request to the API gateway. 

Step 2 - The API gateway parses and validates the attributes in the HTTP request. 

Step 3 - The API gateway performs allow-list/deny-list checks. 

Step 4 - The API gateway talks to an identity provider for authentication and authorization. 

Step 5 - The rate limiting rules are applied to the request. If it is over the limit, the request is rejected. 

Steps 6 and 7 - Now that the request has passed basic checks, the API gateway finds the relevant service to route to by path matching. 

Step 8 - The API gateway transforms the request into the appropriate protocol and sends it to backend microservices. 

Steps 9-12: The API gateway can handle errors properly, and deals with faults if the error takes a longer time to recover (circuit break). It can also leverage ELK (Elastic-Logstash-Kibana) stack for logging and monitoring. We sometimes cache data in the API gateway. 

### How do we design effective and safe APIs?

The diagram below shows typical API designs with a shopping cart example. 

<p>
  <img src="images/safe-apis.jpg" />
</p>


Note that API design is not just URL path design. Most of the time, we need to choose the proper resource names, identifiers, and path patterns. It is equally important to design proper HTTP header fields or to design effective rate-limiting rules within the API gateway. 

### TCP/IP encapsulation 

How is data sent over the network? Why do we need so many layers in the OSI model?
The diagram below shows how data is encapsulated and de-encapsulated when transmitting over the network.

<p>
  <img src="images/osi model.jpeg" />
</p>


Step 1: When Device A sends data to Device B over the network via the HTTP protocol, it is first added an HTTP header at the application layer. 

Step 2: Then a TCP or a UDP header is added to the data. It is encapsulated into TCP segments at the transport layer. The header contains the source port, destination port, and sequence number.

Step 3: The segments are then encapsulated with an IP header at the network layer. The IP header contains the source/destination IP addresses.

Step 4: The IP datagram is added a MAC header at the data link layer, with source/destination MAC addresses.

Step 5: The encapsulated frames are sent to the physical layer and sent over the network in binary bits.

Steps 6-10: When Device B receives the bits from the network, it performs the de-encapsulation process, which is a reverse processing of the encapsulation process. The headers are removed layer by layer, and eventually, Device B can read the data.

We need layers in the network model because each layer focuses on its own responsibilities. Each layer can rely on the headers for processing instructions and does not need to know the meaning of the data from the last layer.


* OSI: open system interconnection
  - does each application has 7 layers or appliation only share layers?
  - overall explanation
    - https://stackoverflow.com/questions/23157817/http-vs-tcp-ip-send-data-to-a-web-server
    - https://www.plixer.com/blog/network-layers-explained/
    - https://www.pearsonitcertification.com/articles/article.aspx?p=1730891
* HTTP header: An HTTP header is a field of an HTTP request or response that passes additional context and metadata about the request or response. For example, a request message can use headers to indicate it's preferred media formats, while a response can use header to indicate the media format of the returned body
* application layer: Two types of software provide access to the network within the application layer
  - https://www.techtarget.com/searchnetworking/definition/Application-layer
  - network-aware applications, such as email; 
  - and application-level services, such as file transfer or print spooling.
* presentation layer: 
  - ensures the information that the application layer of one system sends out is readable by the application layer of another system. On the sending system it is responsible for conversion to standard, transmittable formats. On the receiving system it is responsible for the translation, formatting, and delivery of information for processing or display.
  - why it is not taken care by application layer or session layer? In many widely used applications and protocols no distinction is actually made between the presentation and application layers. For example, HyperText Transfer Protocol (HTTP), generally regarded as an application-layer protocol,
* session layer (rpc socket) https://www.geeksforgeeks.org/session-layer-in-osi-model/
  - enables applications to establish and maintain sessions and to synchronize the sessions. 
  - The ability to send larger amount of data files is extremely important and a necessary thing too.
  - this layer basically provides a mechanism of opening, closing and managing a session between the end-user application processes
  - The services offered by Session Layer are generally implemented in application environments using remote procedure calls (RPCs)
  - so the application controlled/implemented by appliation 
  - session Layer creates procedures for checkpointing followed by adjournment, restart and termination.
  - protocal examples: rpcp, ...
* transportation layer(TCP / UDP) https://www.imperva.com/learn/ddos/tcp-transmission-control-protocol/
  - How should it know which one/program on the receiver side to deliver your message to? 
  - TCP header: source port, dest port, sequence number, 
  - TCP guarantees that bytes are transmitted in the order in which they were sent with no errors or omissions.
  - establish connection: 3 way handshake
  - send data by segments; each of which packaged into datagram and sent to its destination 
* network layer:
  - the IP header contains the source/destination IP addresses.
  - IP is responsible for sending each packet to its destination,
  - setting up the routes for data packets to take, checking to see if a server in another network is up and running, and addressing and receiving IP packets from other networks
* data link layer: https://www.geeksforgeeks.org/data-link-layer/
  - logical link control: divides them into small frames, then, sends each frame bit-by-bit to the next layer
  - media access control: encapsulates the source and destination’s physical address in the header of each frame 
  - data transfer speed/flow control: it’s the responsibility of DLL to synchronize the sender’s and receiver’s speeds and establish flow control between them. 
* physical layer



### Why is Nginx called a “reverse” proxy?

The diagram below shows the differences between a 𝐟𝐨𝐫𝐰𝐚𝐫𝐝 𝐩𝐫𝐨𝐱𝐲 and a 𝐫𝐞𝐯𝐞𝐫𝐬𝐞 𝐩𝐫𝐨𝐱𝐲.

<p>
  <img src="images/Forward Proxy v.s. Reverse Proxy2x.jpg" style="width: 720px" />
</p>

A forward proxy is a server that sits between user devices and the internet.

A forward proxy is commonly used for: 

1. Protecting clients
2. Blocking access to certain content
3. Circumventing browsing restrictions, b/c some proxy has block the access to certani content, so choose different proxy could circumvent

A reverse proxy is a server that accepts a request from the client, forwards the request to web servers, and returns the results to the client as if the proxy server had processed the request.

A reverse proxy is good for:

1. Protecting servers
2. Load balancing
3. Caching static contents
4. Encrypting and decrypting SSL communications

### What are the common load-balancing algorithms?

The diagram below shows 6 common algorithms. 

<p>
  <img src="images/lb-algorithms.jpg" />
</p>

- Static Algorithms (pre-specified rule)

1. Round robin

    The client requests are sent to different service instances in sequential order. The services are usually required to be stateless. 

3. Sticky round-robin

    This is an improvement of the round-robin algorithm. If Alice’s first request goes to service A, the following requests go to service A as well. 

4. Weighted round-robin

    The admin can specify the weight for each service. The ones with a higher weight handle more requests than others. 

6. Hash

    This algorithm applies a hash function on the incoming requests’ IP or URL. The requests are routed to relevant instances based on the hash function result. 

- Dynamic Algorithms (performance based)

5. Least connections

    A new request is sent to the service instance with the least concurrent connections. 

7. Least response time

    A new request is sent to the service instance with the fastest response time.

### URL, URI, URN - Do you know the differences? 

The diagram below shows a comparison of URL, URI, and URN. 

<p>
  <img src="images/url-uri-urn.jpg" />
</p>

- URI 

URI stands for Uniform Resource Identifier. It identifies a logical or physical resource on the web. URL and URN are subtypes of URI. URL locates a resource, while URN names a resource. 

A URI is composed of the following parts: 
scheme:[//authority]path[?query][#fragment] 

- URL 

URL stands for Uniform Resource Locator, the key concept of HTTP. It is the address of a unique resource on the web. It can be used with other protocols like FTP and JDBC. 

- URN 

URN stands for Uniform Resource Name. It uses the urn scheme. URNs cannot be used to locate a resource. A simple example given in the diagram is composed of a namespace and a namespace-specific string. 

If you would like to learn more detail on the subject, I would recommend [W3C’s clarification](https://www.w3.org/TR/uri-clarification/).


## Database

### A nice cheat sheet of different databases in cloud services

<p>
  <img src="images/cloud-dbs2.png" />
</p>

CRUD operations
* Create: Documents can be created in the database. Each document has a unique identifier.
* Read: Documents can be read from the database. The API or query language allows developers to query for documents using their unique identifiers or field values. Indexes can be added to the database in order to increase read performance.
* Update: Existing documents can be updated — either in whole or in part.
* Delete: Documents can be deleted from the database.

* structured 
  - relational: 
    - aws: RDS
    - Oracle
    - postgreSQL
    - MySQL
  - columnar: https://thenewstack.io/what-is-a-column-database-and-when-should-you-use-one/
    - It has seven different tables, one for each Person attribute, such as Person.Height. Each table has two columns: The piece of data they're storing and a Person ID.
      - it is less work to go through Person.Heights table
      - columnar db often maintain useful stats
    - use case and advantage
      - optimized
        - better compression due to the same data type of each column
        - store multiple version of the same col
        - adaptive index / vectorize processing
      - trade off
        - update / write individual data point => write/update in batch
        - if read all columns of rows
    - aws: redshift
    - snowflake
* semi structured
  - key-value
    - aws: dynamoDB
    - redis (Remote Dictionary Server.):
      - how to install/start
        - brew install redis
        - redis-server
        - redis-cli
      - how to represent table: with colums? use hahses (https://redis.io/docs/get-started/data-store/)
        - use primary key as hash: and store the rest of the {col:val} into object => only fetch by primary key
        - if want to filter by other columns, which are not primary/unique key: could use set 
          - https://redis.io/docs/data-types/sets/
          - sadd other_col:value primary_col:value # there is set name:= other_col:value and member
          - smembers other_col:value => all primary_col:values # if it is common key => redis max size = 2^32 ~ 4,294,967,295
      - get|set: are used to store/fetch simple strings: if it is stored as SET, has to fetch by GET, otherwise  ERR wrong number of arguments for 'hget' command
      - hset|hget: are used to store objects; 1). the object has to be even => dict; otherwise ERR wrong number of arguments for 'hset' command
    - memcache: 
      - https://www.dragonflydb.io/guides/memcached
      - https://www.tutorialspoint.com/memcached/memcached_incr_decr.htm
  - wide column (https://db-engines.com/en/article/Wide+Column+Stores)
    - a record can have billions of columns => can be seen as two-dimensional key-value stores. which is the reason of called "wide column DB"
    - aws: keyspaces
    - HBase: 
    - cassandra 
      - install: https://www.javatpoint.com/how-to-install-cassandra-on-mac;
      - run: export JAVA_HOME=$(/usr/libexec/java_home -v 1.8), then run cassandra -f => service started; then run cqlsh localhost in another terminal; 
      - use: https://www.datastax.com/blog/working-apache-cassandra-mac-os-x
      - use cases: https://www.datastax.com/blog/exploring-common-apache-cassandra-use-cases
      - based on ideas of BigTable and DynamoDB
      - Cassandra has the concept of a keyspace, which is similar to a database in a RDBMS
      - meaning that rows in a column family can have different columns depending on the data you want to store for a particular row
        - could add column incrementally, alter table add (new_col type);
        - the missing column will be null;
        - should not use * to query all columns, but instead should specify the desired columns
      - if you want to query columns other than the primary key, you need to create a secondary index on them:
  - in-memory
    - aws: elastCache
    - redis
    - memcache
  - time series
  - immutable ledger
  - gepspatial
  - graph
  - document
    - A document typically stores information about one object and any of its related metadata, Documents can be stored in formats like JSON, BSON, and XML.
    - A collection is a group of documents. Collections typically store documents that have similar contents. Not all document has the same filed
    - why document db
      - Low Performance on json data
      - json data validation
      - addtional vendor language to support json
      - no native scale out
    - aws: documentDB
    - MongoDB (https://www.mongodb.com/document-databases)
      - https://www.mongodb.com/docs/manual/reference/method/db.collection.insertMany/
      - databases, collections, documents; language similar to graph query
      - Fields in a document play the role of columns in a SQL database, and like columns, they can be indexed to increase search performance.
      - use cases
        - describing complex data
        - integration large amount of diverse data => flexible of bring data together
      - scaling https://www.mongodb.com/basics/scaling
        - replication
          - it native make the system more resilient to node failer, but 
          - increase read from nodes
          - write to primry
        - sharding
          - more complex scaling, client application connects to a sharded cluster through a router that directs the requests to the appropriate nodes.
    - couchbase
  - text search
* unstructured : blob
  - aws: s3
  - 


Use cases
* DB + memcache => Cassandra
  - Cassandra provides both durable storage, and an integrated, high performance cache (the "row cache"). 
  - This prevents problems like memcached being populated from an out of date slave (what Twitter calls "potential consistency") and simplifies cluster management.


Choosing the right database for your project is a complex task. Many database options, each suited to distinct use cases, can quickly lead to decision fatigue. 

We hope this cheat sheet provides high-level direction to pinpoint the right service that aligns with your project's needs and avoid potential pitfalls. 

Note: Google has limited documentation for their database use cases. Even though we did our best to look at what was available and arrived at the best option, some of the entries may need to be more accurate. 

### 8 Data Structures That Power Your Databases
General data strcture in terms of storage format
* Seq based: Array
* Pointer based: linkedList, tree, graph

The answer will vary depending on your use case. Data can be indexed in memory or on disk. Similarly, data formats vary, such as numbers, strings, geographic coordinates, etc. The system might be write-heavy or read-heavy. All of these factors affect your choice of database index format. 

<p>
  <img src="images/8-ds-db.jpg" />
</p>

The following are some of the most popular data structures used for indexing data: 
- Hash index: a very common implementation of the “Map” data structure (or 
- Skiplist: a common in-memory index type. Used in Redis;  
  - its insert/removal, are log(n); if we add skip lenght => random access could also be improved to log(n)
  - sorted array: search/lookup is O(1), but insert/removal is O(n) due to its data structure; 
  - sorted double linked list: search/lookup is O(n), but insert/removal is O(1) due to its data structure; 
  - used by redis/ in memory
    - extra space: p + p^2 + 1 = 1/(1-p) times for space
    - how many layers: while num of node in layer j > 1, 
  - how to implement
“Collection”) 
- SSTable: immutable on-disk “Map” implementation;  used for document storage
  - is a persistent file format used by ScyllaDB, Apache Cassandra, and other NoSQL databases to take the in-memory data stored in memtables, order it for fast access, and store it on disk in a persistent, ordered, immutable set of files
  - An SSTable provides a persistent,ordered immutable map from keys to values, where both keys and values are arbitrary byte strings. Operations are provided to look up the value associated with a specified key, and to iterate over all key/value pairs in a specified key range. 
  - Internally, each SSTable contains a sequence of blocks (typically each block is 64KB in size, but this is configurable). A block index (stored at the end of the SSTable) is used to locate blocks; the index is loaded into memory when the SSTable is opened. A lookup can be performed with a single disk seek: we first find the appropriate block by performing a binary search in the in-memory index, and then reading the appropriate block from disk. Optionally, an SSTable can be completely mapped into memory, which allows us to perform lookups and scans without touching disk.
  - value in sstable: store the offset; where file is stored in a big continuous accessible disk
- LSM tree: Skiplist + SSTable. High write throughput (ref: https://blog.devgenius.io/understanding-lsm-log-structured-merge-trees-4bf77777fef4)
  - example 
    - back system <p><img src="images/lsmt_system_img.webp"></p>; 
    - used in Apache Cassandra and LevelDB, 
  - components
    - bloom filter: for write/request, check whether data in disk (sstable)
    - WAL(write ahead log): which is a sequential write append log on disk. to improve the durability; != directly write to disk, which is random disk I/O; Open a file and append it, is it a sequential access? 
    - memtable: used to store recently modified data, help efficient/ low-latency write operations; it can be implemented by skiplist; off-heap memory(not subject to java GC). 
    - sstable: which is optimized for range query; as keys are sorted; b/c sstable is immutable data structure, once stored it will not be modified. any modification/delete => new sstable; 
      - the sort key could be timestamp; 
      - key creation: top level := most recent; bottom level with the older data
      - periodic merge process: select(size, age, overlapping key range)
- B-tree: disk-based solution. Consistent read/write performance 
  - comapre with balck-red(binary version): internal node also hold data; and store data more efficiently
  - compared with skip-list:
    - B-tree: 
      - more efficient 
      - small overhead per key (internal node could store multiple keys)
      - but complex to implement
      - challenging in lock-free or concurrent to ensure atomicity during structural modifications
    - skiplist
      - easier to implement in lock-free or concurrent scenarios
      - probabilistic 
  - why it is used in disk based index? 
    - each node has multiple key
      - for sequential access which is important for disk I/O
      - read relatively fewer blocks
      - range queries
    - balanceness
      - handle large database
      - cache efficiency
    - predictable performance
- Inverted index: used for document indexing. Used in Lucene 
  - used in lucenne/elastic search (not traditional db)
- Suffix tree: for string pattern search 
- R-tree: multi-dimension search, such as finding the nearest neighbor 

### How is an SQL statement executed in the database?

The diagram below shows the process. Note that the architectures for different databases are different, the diagram demonstrates some common designs.

<p>
  <img src="images/sql execution order in db.jpeg" style="width: 580px" />
</p>


Step 1 - A SQL statement is sent to the database via a transport layer protocol (e.g.TCP).

Step 2 - The SQL statement is sent to the command parser, where it goes through syntactic and semantic analysis, and a query tree is generated afterward.

Step 3 - The query tree is sent to the optimizer. The optimizer creates an execution plan. 

Step 4 - The execution plan is sent to the executor. The executor retrieves data from the execution.

Step 5 - Access methods provide the data fetching logic required for execution, retrieving data from the storage engine. 

Step 6 - Access methods decide whether the SQL statement is read-only. If the query is read-only (SELECT statement), it is passed to the buffer manager for further processing. The buffer manager looks for the data in the cache or data files.

Step 7 - If the statement is an UPDATE or INSERT, it is passed to the transaction manager for further processing.

Step 8 - During a transaction, the data is in lock mode. This is guaranteed by the lock manager. It also ensures the transaction’s ACID properties. 

##### SQL topic summary
  - establish connection between client and database server 
  - example protocal JDBC: does not define protocol, rely on underlying database-specific drivers to communicate with the databases. 
    - type-4 thin driver'
    - it does not dffine a specific protocol, it provides standardized API
  - execuation
    - read only: buffer manager, cache/data files
    - transaction: transaction manager a). data is in lock mode by lock manager; b). ensure the ACID properties,  which are 
      - atomicity: as single, not further divisible 
      - consistency: preserve integrity constraints and business rules; money taken then all copies could realized the change
      - isolation: one transaction will not affect other transactions
      - durability: transaction committed will be permanent, will stay the same with system failure 

  - data transfer
    - data serialization in binary format or json or xml for easy transmit and reconstruction
    - database specific protocal


###  CAP theorem

The CAP theorem is one of the most famous terms in computer science, but I bet different developers have different understandings. Let’s examine what it is and why it can be confusing. 

<p>
  <img src="images/cap theorem.jpeg" />
</p>

CAP theorem states that a **distributed system** can't provide more than two of these three guarantees simultaneously.

**Consistency**: consistency means all clients see the same data at the same time no matter which node they connect to.

**Availability**: availability means any client that requests data gets a response even if some of the nodes are down. A continuous measurement of availability is latency.

**Partition Tolerance**: a partition indicates a communication break between two nodes. Partition tolerance means the system continues to operate despite network partitions. 

The “2 of 3” formulation can be useful, **but this simplification could be misleading**.

1. Picking a database is not easy. Justifying our choice purely based on the CAP theorem is not enough. For example, companies don't choose Cassandra for chat applications simply because it is an AP system. There is a list of good characteristics that make Cassandra a desirable option for storing chat messages. We need to dig deeper.

2. “CAP prohibits only a tiny part of the design space: perfect availability and consistency in the presence of partitions, which are rare”. Quoted from the paper: CAP Twelve Years Later: How the “Rules” Have Changed.

3. The theorem is about 100% availability and consistency. A more realistic discussion would be the trade-offs between latency(how long it take to populate changes to all nodes, long latency=not available) and consistency when there is no network partition. See PACELC theorem for more details.

**Is the CAP theorem actually useful?**

I think it is still useful as it opens our minds to a set of tradeoff discussions, but it is only part of the story. We need to dig deeper when picking the right database.

**EXAMPE**
* CA system: single node, does not tolerant partition; single node database
* CP systems: strong consitency required, used in banks, financial system; zookeeper, big table
* AP systems: does not have to be consistent, but need to be available or low latency for purpose of user experience
  - DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services (AWS). It is designed for high availability and scalability. DynamoDB is often classified as an AP system because it prioritizes availability and partition tolerance, allowing for continuous operation in the face of network partitions. It provides eventual consistency by default but also allows users to configure stronger consistency if needed.
  - Apache Cassandra is an open-source, distributed NoSQL database that is designed for high availability and scalability. It follows a peer-to-peer architecture and is known for its ability to scale horizontally across multiple nodes. Cassandra is classified as an AP system because it prioritizes availability and partition tolerance over strong consistency.
  - Redis is an in-memory data store that can be used for caching, session storage, and more. While Redis is often used for its speed and simplicity, when configured for high availability using Redis Sentinel or Redis Cluster, it becomes more of an AP system. It prioritizes availability and may provide eventual consistency
    - it is master-slave;
      - slave read only
      - min-replicas-to-write to consider as successful write 
      - control the durability: write to disk, no, every_second, always
      - sentinal: monitor; if one master fail, promote one of its replica for availability
    - data partition: use data partition across multiple nodes, each responsible for a subset of data; could scale horizontally. 
    - async replication, from master node to its replica; 
    - used in high performance use case, like cache, session storage, real-time analystics, message queuee. 
    - conflict resolution: last-write-wins
  - CouchDB is an open-source NoSQL database that uses a document-oriented model. It is designed for ease of replication and distribution. CouchDB is often considered an AP system because it prioritizes availability and allows for flexible, eventually consistent replication across nodes.
  - Amazon S3 is a scalable object storage service that provides high availability and durability for storing and retrieving data. S3 is designed to be highly available even in the face of network partitions, making it an AP system. It provides eventual consistency for read-after-write scenarios.


### Types of Memory and Storage

<p>
  <img src="images/Types_of_Memory_and_Storage.jpeg" style="width: 420px" />
</p>

* memory
  - rom
  - RAM
    - SRAM (Static Random Access Memory), faster and low latency, often used for cache memory
    - DRAM (Dynamic Random Access Memory), need periodic refreshing
* storage

### Visualizing a SQL query

<p>
  <img src="images/sql-execution-order.jpg" style="width: 580px" />
</p>

SQL statements are executed by the database system in several steps, including: 

- Parsing the SQL statement and checking its validity 
- Transforming the SQL into an internal representation, such as relational algebra 
- Optimizing the internal representation and creating an execution plan that utilizes index information 
- Executing the plan and returning the results 

The execution of SQL is highly complex and involves many considerations, such as: 

- The use of indexes and caches 
- The order of table joins 
- Concurrency control 
- Transaction management 

### SQL language 

In 1986, SQL (Structured Query Language) became a standard. Over the next 40 years, it became the dominant language for relational database management systems. Reading the latest standard (ANSI SQL 2016) can be time-consuming. How can I learn it? 

<p>
  <img src="images/how-to-learn-sql.jpg" />
</p>

There are 5 components of the SQL language: 

- DDL: data definition language, such as CREATE, ALTER, DROP 
- DQL: data query language, such as SELECT 
- DML: data manipulation language, such as INSERT, UPDATE, DELETE 
- DCL: data control language, such as GRANT, REVOKE 
- TCL: transaction control language, such as COMMIT, ROLLBACK 

For a backend engineer, you may need to know most of it. As a data analyst, you may need to have a good understanding of DQL. Select the topics that are most relevant to you. 

## Cache

### Data is cached everywhere

This diagram illustrates where we cache data in a typical architecture.

<p>
  <img src="images/where do we cache data.jpeg" style="width: 720px" />
</p>


There are **multiple layers** along the flow.

1. Client apps: HTTP responses can be cached by the browser. We request data over HTTP for the first time, and it is returned with an expiry policy in the HTTP header; we request data again, and the client app tries to retrieve the data from the browser cache first.
  * one site could have multiple cookie with different values, for example uuid, country, with different expiration, as it would take some resrouce to generate these values

2. CDN: CDN caches static web resources. The clients can retrieve data from a CDN node nearby.
  * components
    - where the content from: origin server/data center, the authoritive of data source
    - edge servers: as caching proxies, storing copies of web contenct closer to end users
    - caching
    - load balancing: cross multiple edge servers, so that no single server become overload
    - scalability/security
    - it does not design to handle write request
    - how to handle dynamic content: based on request, edge server computing
    
3. Load Balancer: The load Balancer can cache resources as well.
4. Messaging infra: Message brokers store messages on disk first, and then consumers retrieve them at their own pace. Depending on the retention policy, the data is cached in Kafka clusters for a period of time.
5. Services: There are multiple layers of cache in a service. If the data is not cached in the CPU cache, the service will try to retrieve the data from memory. Sometimes the service has a second-level cache to store data on disk.
6. Distributed Cache: Distributed cache like Redis holds key-value pairs for multiple services in memory. It provides much better read/write performance than the database.
7. Full-text Search: we sometimes need to use full-text searches like Elastic Search for document search or log search. A copy of data is indexed in the search engine as well.
8. Database: 
  * Even in the database, we have different levels of caches:
    - WAL(Write-ahead Log): data is written to WAL first before building the B tree index
    - Bufferpool: A memory area allocated to cache query results
    - Materialized View: Pre-compute query results and store them in the database tables for better query performance
    - Transaction log: record all the transactions and database updates
    - Replication Log: used to record the replication state in a database cluster

### Why is Redis so fast? 

There are 3 main reasons as shown in the diagram below.
https://www.linkedin.com/pulse/why-heck-single-threaded-redis-lightning-fast-beyond-in-memory-kapur 

<p>
  <img src="images/why_redis_fast.jpeg" />
</p>


1. Redis is a RAM-based data store. RAM access is at least 1000 times faster than random disk access.
  * 120 ns
    - ssd 120 us
    - HDD 1-10 ms
2. Redis leverages IO multiplexing and single-threaded execution loop for execution efficiency. 
  * using single thread to monitoring multiple client connections(each connection has an associated thread)
    - if multiple thread do IO => increase memory overhead, thread synchronization overhead (lock), context switch
    - single thread to achieve, by using OS provied system calls like "select, pool, epoll", which allow the application to wait for events on multiple I/O streams
  * single threaded architecture, where all cmd exe in sequential order
    - atomic and consitency and avoid race condition
  * all clients to send multiple request
3. Redis leverages several efficient lower-level data structures.
  * index: skiplist, hashmap

4. build distributed cache with redis (https://stackoverflow.com/questions/18376665/redis-distributed-or-not)
  * Q1 single machine has cap on redis capacity: 
  * Q2 is redis a distributed system or not: 
    - sentinal only cover role management, side effect improve availability 
    - build AP: write to master, but read from all instance
    - build CP: always conntec to master  
    - sharding vs. master/slave
  * conclusion: If you need an off-the-shelf distributed store, Redis is probably not a good option. You will be better served by Cassandra, Riak, MongoDB, Couchbase, Aerospike, MySQL Cluster, Oracle NoSQL, etc ... However, if you want to build your own specialized system, Redis is an excellent component to build upon.
  * new version of redis: https://redis.io/docs/management/scaling/
    - scalability sharding  based on hashing
    - availability replica
  

Question: Another popular in-memory store is Memcached. Do you know the differences between Redis and Memcached?
https://aws.amazon.com/elasticache/redis-vs-memcached/
* redis is more rich features
* memcached for simplicity 

You might have noticed the style of this diagram is different from my previous posts. Please let me know which one you prefer.

### How can Redis be used?

<p>
  <img src="images/top-redis-use-cases.jpg" style="width: 520px" />
</p>


There is more to Redis than just caching. 

Redis can be used in a variety of scenarios as shown in the diagram. 

- Session 

  We can use Redis to share user session data among different services. 

- Cache 

  We can use Redis to cache objects or pages, especially for hotspot data. 

- Distributed lock 

  We can use a Redis string to acquire locks among distributed services. 

- Counter 

  We can count how many likes or how many reads for articles. 

- Rate limiter 

  We can apply a rate limiter for certain user IPs. 

- Global ID generator 

  We can use Redis Int for global ID. 

- Shopping cart 

  We can use Redis Hash to represent key-value pairs in a shopping cart. 

- Calculate user retention 

  We can use Bitmap to represent the user login daily and calculate user retention. 

- Message queue 

  We can use List for a message queue. 

- Ranking 

  We can use ZSet to sort the articles. 

### Top caching strategies

Designing large-scale systems usually requires careful consideration of caching. 
Below are five caching strategies that are frequently utilized. 
1. cache side: application responsible for cache update after read
2. read through: check cache, if miss query db, then update cache, then return to client from cache
3. write back: write to cache first, then write to DB
  - back: to db once for a while
  - through: to db immediately

<p>
  <img src="images/top_caching_strategy.jpeg" style="width: 680px" />
</p>


## Payment systems

### How to learn payment systems?

<p>
  <img src="images/learn-payments.jpg" />
</p>

###  Why is the credit card called “the most profitable product in banks”? How does VISA/Mastercard make money? 

The diagram below shows the economics of the credit card payment flow.

<p>
  <img src="images/how does visa makes money.jpg" style="width: 640px" />
</p>

1.&nbsp;&nbsp;The cardholder pays a merchant $100 to buy a product.

2.&nbsp;The merchant benefits from the use of the credit card with higher sales volume and needs to compensate the issuer and the card network for providing the payment service. The acquiring bank sets a fee with the merchant, called the “merchant discount fee.”

3 - 4. The acquiring bank keeps $0.25 as the acquiring markup, and $1.75 is paid to the issuing bank as the interchange fee. The merchant discount fee should cover the interchange fee. 

  The interchange fee is set by the card network because it is less efficient for each issuing bank to negotiate fees with each merchant.

5.&nbsp;&nbsp;The card network sets up the network assessments and fees with each bank, which pays the card network for its services every month. For example, VISA charges a 0.11% assessment, plus a $0.0195 usage fee, for every swipe.

6.&nbsp;&nbsp;The cardholder pays the issuing bank for its services.

Why should the issuing bank be compensated?

- The issuer pays the merchant even if the cardholder fails to pay the issuer. 
- The issuer pays the merchant before the cardholder pays the issuer.
- The issuer has other operating costs, including managing customer accounts, providing statements, fraud detection, risk management, clearing & settlement, etc. 

### How does VISA work when we swipe a credit card at a merchant’s shop?

<p>
  <img src="images/visa_payment.jpeg" />
</p>


VISA, Mastercard, and American Express act as card networks for the clearing and settling of funds. The card acquiring bank and the card issuing bank can be – and often are – different. If banks were to settle transactions one by one without an intermediary, each bank would have to settle the transactions with all the other banks. This is quite inefficient.   
 
The diagram below shows VISA’s role in the credit card payment process. There are two flows involved. Authorization flow happens when the customer swipes the credit card. Capture and settlement flow happens when the merchant wants to get the money at the end of the day.
 
- Authorization Flow

Step 0: The card issuing bank issues credit cards to its customers. 
 
Step 1: The cardholder wants to buy a product and swipes the credit card at the Point of Sale (POS) terminal in the merchant’s shop.
 
Step 2: The POS terminal sends the transaction to the acquiring bank, which has provided the POS terminal.
 
Steps 3 and 4: The acquiring bank sends the transaction to the card network, also called the card scheme. The card network sends the transaction to the issuing bank for approval.
 
Steps 4.1, 4.2 and 4.3: The issuing bank freezes the money if the transaction is approved. The approval or rejection is sent back to the acquirer, as well as the POS terminal. 
 
- Capture and Settlement Flow

Steps 1 and 2: The merchant wants to collect the money at the end of the day, so they hit ”capture” on the POS terminal. The transactions are sent to the acquirer in batch. The acquirer sends the batch file with transactions to the card network.
 
Step 3: The card network performs clearing for the transactions collected from different acquirers, and sends the clearing files to different issuing banks.
 
Step 4: The issuing banks confirm the correctness of the clearing files, and transfer money to the relevant acquiring banks.
 
Step 5: The acquiring bank then transfers money to the merchant’s bank. 
 
Step 4: The card network clears up the transactions from different acquiring banks. Clearing is a process in which mutual offset transactions are netted, so the number of total transactions is reduced.
 
In the process, the card network takes on the burden of talking to each bank and receives service fees in return.

### Payment Systems Around The World Series (Part 1): Unified Payments Interface (UPI) in India


What’s UPI? UPI is an instant real-time payment system developed by the National Payments Corporation of India.

It accounts for 60% of digital retail transactions in India today.

UPI = payment markup language + standard for interoperable payments


<p>
  <img src="images/how-does-upi-work.png"  style="width: 600px" />
</p>


## CI/CD

### CI/CD Pipeline Explained in Simple Terms

<p>
  <img src="images/ci-cd-pipeline.jpg" style="width: 680px" />
</p>

Section 1 - SDLC with CI/CD

The software development life cycle (SDLC) consists of several key stages: development, testing, deployment, and maintenance. CI/CD automates and integrates these stages to enable faster and more reliable releases.

When code is pushed to a git repository, it triggers an automated build and test process. End-to-end (e2e) test cases are run to validate the code. If tests pass, the code can be automatically deployed to staging/production. If issues are found, the code is sent back to development for bug fixing. This automation provides fast feedback to developers and reduces the risk of bugs in production.

Section 2 - Difference between CI and CD

Continuous Integration (CI) automates the build, test, and merge process. It runs tests whenever code is committed to detect integration issues early. This encourages frequent code commits and rapid feedback.

Continuous Delivery (CD) automates release processes like infrastructure changes and deployment. It ensures software can be released reliably at any time through automated workflows. CD may also automate the manual testing and approval steps required before production deployment.

Section 3 - CI/CD Pipeline

A typical CI/CD pipeline has several connected stages:
- The developer commits code changes to the source control
- CI server detects changes and triggers the build
- Code is compiled, and tested (unit, integration tests)
- Test results reported to the developer
- On success, artifacts are deployed to staging environments
- Further testing may be done on staging before release
- CD system deploys approved changes to production

### Netflix Tech Stack (CI/CD Pipeline)

<p>
  <img src="images/netflix-ci-cd.jpg" style="width: 720px" />
</p>

Planning: Netflix Engineering uses JIRA for planning and Confluence for documentation. 

Coding: Java is the primary programming language for the backend service, while other languages are used for different use cases.  

Build: Gradle is mainly used for building, and Gradle plugins are built to support various use cases.  

Packaging: Package and dependencies are packed into an Amazon Machine Image (AMI) for release. 

Testing: Testing emphasizes the production culture's focus on building chaos tools.  

Deployment: Netflix uses its self-built Spinnaker for canary rollout deployment.  

Monitoring: The monitoring metrics are centralized in Atlas, and Kayenta is used to detect anomalies.  

Incident report: Incidents are dispatched according to priority, and PagerDuty is used for incident handling. 


## DevOps

###  DevOps vs. SRE vs. Platform Engineering. What is the difference?

The concepts of DevOps, SRE, and Platform Engineering have emerged at different times and have been developed by various individuals and organizations. 

<p>
  <img src="images/devops-sre-platform.jpg" />
</p>

DevOps as a concept was introduced in 2009 by Patrick Debois and Andrew Shafer at the Agile conference. They sought to bridge the gap between software development and operations by promoting a collaborative culture and shared responsibility for the entire software development lifecycle. 

SRE, or Site Reliability Engineering, was pioneered by Google in the early 2000s to address operational challenges in managing large-scale, complex systems. Google developed SRE practices and tools, such as the Borg cluster management system and the Monarch monitoring system, to improve the reliability and efficiency of their services. 

Platform Engineering is a more recent concept, building on the foundation of SRE engineering. The precise origins of Platform Engineering are less clear, but it is generally understood to be an extension of the DevOps and SRE practices, with a focus on delivering a comprehensive platform for product development that supports the entire business perspective. 

It's worth noting that while these concepts emerged at different times. They are all related to the broader trend of improving collaboration, automation, and efficiency in software development and operations. 

### What is k8s (Kubernetes)?

K8s is a container orchestration system. It is used for container deployment and management. Its design is greatly impacted by Google’s internal system Borg.

<p>
  <img src="images/k8s.jpeg" style="width: 680px" />
</p>

A k8s cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node.

The worker node(s) host the Pods that are the components of the application workload. The control plane manages the worker nodes and the Pods in the cluster. In production environments, the control plane usually runs across multiple computers, and a cluster usually runs multiple nodes, providing fault tolerance and high availability.

- Control Plane Components

1. API Server

    The API server talks to all the components in the k8s cluster. All the operations on pods are executed by talking to the API server.

2. Scheduler

    The scheduler watches pod workloads and assigns loads on newly created pods.

3. Controller Manager

    The controller manager runs the controllers, including Node Controller, Job Controller, EndpointSlice Controller, and ServiceAccount Controller.

4. Etcd
    
    etcd is a key-value store used as Kubernetes' backing store for all cluster data.

- Nodes

1. Pods

    A pod is a group of containers and is the smallest unit that k8s administers. Pods have a single IP address applied to every container within the pod.

2. Kubelet

    An agent that runs on each node in the cluster. It ensures containers are running in a Pod.

3. Kube Proxy

    Kube-proxy is a network proxy that runs on each node in your cluster. It routes traffic coming into a node from the service. It forwards requests for work to the correct containers.

### Docker vs. Kubernetes. Which one should we use? 

<p>
  <img src="images/docker-vs-k8s.jpg" style="width: 680px" />
</p>


What is Docker ? 

Docker is an open-source platform that allows you to package, distribute, and run applications in isolated containers. It focuses on containerization, providing lightweight environments that encapsulate applications and their dependencies. 

What is Kubernetes ? 

Kubernetes, often referred to as K8s, is an open-source container orchestration platform. It provides a framework for automating the deployment, scaling, and management of containerized applications across a cluster of nodes. 

How are both different from each other ? 

Docker: Docker operates at the individual container level on a single operating system host. 

You must manually manage each host and setting up networks, security policies, and storage for multiple related containers can be complex. 

Kubernetes: Kubernetes operates at the cluster level. It manages multiple containerized applications across multiple hosts, providing automation for tasks like load balancing, scaling, and ensuring the desired state of applications. 

In short, Docker focuses on containerization and running containers on individual hosts, while Kubernetes specializes in managing and orchestrating containers at scale across a cluster of hosts. 

### How does Docker work? 

The diagram below shows the architecture of Docker and how it works when we run “docker build”, “docker pull” 
and “docker run”. 

<p>
  <img src="images/docker.jpg" style="width: 680px" />
</p>

There are 3 components in Docker architecture: 

- Docker client 
    
    The docker client submit cmd, to the Docker daemon, host will decide if it is necessary to connect registry.
    It provides a command line interface (CLI) that allows you to issue build, run, and stop application commands to a Docker daemon. 
    It connects host and registry. 

- Docker host 

    The Docker daemon listens for Docker API requests and manages Docker objects such as images, containers, networks, and volumes. 
    Will container run on the host? 

- Docker registry 

    A Docker registry stores Docker images. Docker Hub is a public registry that anyone can use. 

Docker objects
- image
- container
- network
- volumes

Let’s take the “docker run” command as an example. 

  1. Docker pulls the image from the registry. 
  1. Docker creates a new container. 
  1. Docker allocates a read-write filesystem to the container. 
  1. Docker creates a network interface to connect the container to the default network. 
  1. Docker starts the container.


Learn kubenetes
* overall walk through example: https://kubernetes.io/docs/tutorials/hello-minikube/
  - explose app
  - scaling: by chance number of replica
    - with scaling, do we still need load-balancer within kubenetes?
    - multiple kubenete behiind real load balancer?
* install 
  - kubectl: curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/darwin/amd64/kubectl"
  - curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/darwin/amd64/kubectl.sha256"
  - sudo mv ./kubectl /usr/local/bin/kubectl
  - kubectl cluster-info # which does not work
  - minikube: curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64
  - kubectl completion zsh
  - minikube start => kubectl is now configured to use "minikube" cluster and "default" namespace by default
  - then "kubectl get po -A" works
  - minikube dashboard # open local webpage
* kubenete action resource
  - kubectl: kubenete api to interact with the cluster
  - actions
    - create (to create deployment)
    - log: print log info from a container in pad
    - delete (to delete service)
    - get (pods, nodes, deployments, etc): to list resources
      - get based on label: kubectl get pods -l label_name=label_value
    - describe: detail info about a resources
    - exec: 
      - execute a command on a container in a pod (必须要这个container support 的command 么？)
      - get all containers on a pod: kubectl get pods pod_name_here -o jsonpath='{.spec.containers[*].name}' (https://stackoverflow.com/questions/33924198/how-do-you-cleanly-list-all-the-containers-in-a-kubernetes-pod)
      - see details on https://kubernetes.io/docs/tutorials/kubernetes-basics/explore/explore-intro/
      - list env variables: kubectl exec "$POD_NAME" -- env
      - run bash on the container: kubectl exec -ti $POD_NAME -- bash ==> after it is running: cat server.js
    - expose, To create a new service and expose it to external traffic we'll use the expose command with NodePort as parameter.
      - parameter: deployment/deployment_name; type, port
    - proxy: a connection between our host (the terminal) and the Kubernetes cluster. The proxy enables direct access to the API from these terminals.
      - with kubectl proxy, terminal could connect to cluster
      - get pod name by "export POD_NAME=$(kubectl get pods -o go-template --template '{{range .items}}{{.metadata.name}}{{"\n"}}{{end}}')"
      - connect to pod by "curl http://localhost:8001/api/v1/namespaces/default/pods/$POD_NAME/"
    - label: to tag a new label to a existing pod
    - scale: "kubectl scale deployments/kubernetes-bootcamp --replicas=1"
  - resources
    - pods
      - shared resources: storage (volumns), networking, 
      - A Pod models an application-specific "logical host" and can contain different application containers which are relatively tightly coupled;(怎么把tightly coupled 的container 放在一起? ); as pod create when deployment, 是不是可以deployment 的时候 有多个container
      - atomic unit on the Kubernetes platform
      - created when we deployment, there is label
    - nodes: a VM or a physical computer that serves as a worker machine
      - kubelet: an agent for managing the node and communicating with the Kubernetes control plane
      - container runtime
      - multiple nodes: otherwise an etcd member and a control plane instance are lost
    - deployments: instructs Kubernetes how to create and update instances of your application
      - "kubectl create deployment deployment_name --image=xxxx"
      - in the controller panel, will create have a deployment object (which include a deployment controller), deployment controller will monitor the instance
      - it will create instance for the app in a node
      - need: 1). container image, 2). number of replica;
      - will create pod, container both?
    - service (which is result of expose command)
      - "kubectl explose deployment/deployment_name"
      - A Service routes traffic across a set of Pods
      - service type: clusterIP, nodePort, loadBalancer (https://stackoverflow.com/questions/41509439/whats-the-difference-between-clusterip-nodeport-and-loadbalancer-service-types?rq=2)
      - match a set of Pods using labels and selectors
    - label (key/value pair for pods, one pod could have multiple labels)
      - "kubectl label pods "$POD_NAME" version=v1" to create new label to a pod
    
* create a kubenetes cluster
  - control panel: coordinates all activities in your cluster, such as scheduling applications, maintaining applications' desired state, scaling applications, and rolling out new updates.
    - kube-apiserver
    - etcd
    - kube-scheduler
    - kube-controller-manager
    - cloud-controller-manager
  - node: 
    
* deploy an app
* explore your app
* expose your app publically
* scale up your app
* update your app

Learn docker


## GIT

### How Git Commands work

To begin with, it's essential to identify where our code is stored. The common assumption is that there are only two locations - one on a remote server like Github and the other on our local machine. However, this isn't entirely accurate. Git maintains three local storages on our machine, which means that our code can be found in four places: 

<p>
  <img src="images/git-commands.png" style="width: 600px" />
</p>


- Working directory: where we edit files 
- Staging area: a temporary location where files are kept for the next commit 
- Local repository: contains the code that has been committed 
- Remote repository: the remote server that stores the code 

Most Git commands primarily move files between these four locations. 

### How does Git Work?

The diagram below shows the Git workflow. 

<p>
  <img src="images/git-workflow.jpeg" style="width: 520px" />
</p>


Git is a distributed version control system. 

Every developer maintains a local copy of the main repository and edits and commits to the local copy. 

The commit is very fast because the operation doesn’t interact with the remote repository. 

If the remote repository crashes, the files can be recovered from the local repositories. 

### Git merge vs. Git rebase

What are the differences?

<p>
  <img src="images/git-merge-git-rebase.jpeg" style="width: 680px" />
</p>


When we **merge changes** from one Git branch to another, we can use ‘git merge’ or ‘git rebase’. The diagram below shows how the two commands work.

**Git merge**

This creates a new commit G’ in the main branch. G’ ties the histories of both main and feature branches.

Git merge is **non-destructive**. Neither the main nor the feature branch is changed.

**Git rebase**

Git rebase moves the feature branch histories to the head of the main branch. It creates new commits E’, F’, and G’ for each commit in the feature branch.

The benefit of rebase is that it has a linear **commit history**.

Rebase can be dangerous if “the golden rule of git rebase” is not followed.

**The Golden Rule of Git Rebase**

Never use it on public branches! (https://stackoverflow.com/questions/2046638/use-of-git-rebase-in-public-feature-branches)

## Cloud Services

### A nice cheat sheet of different cloud services (2023 edition)

<p>
  <img src="images/cloud-compare.jpg" />
</p>


### What is cloud native?

Below is a diagram showing the evolution of architecture and processes since the 1980s. 

<p>
  <img src="images/cloud-native.jpeg" style="width: 640px" />
</p>

Organizations can build and run scalable applications on public, private, and hybrid clouds using cloud native technologies. 

This means the applications are designed to leverage cloud features, so they are resilient to load and easy to scale. 

Cloud native includes 4 aspects: 

1. Application Architecture 

    The architecture has gone from monolithic to microservices. Each service is designed to be small, adaptive to the limited resources in cloud containers. 

2. Development process 

    This has progressed from waterfall to agile to DevOps. 

3. Deployment & packaging 

    The applications used to be deployed on physical servers. Then around 2000, the applications that were not sensitive to latency were usually deployed on virtual servers. With cloud native applications, they are packaged into docker images and deployed in containers. 

4. Application infrastructure 

    The applications are massively deployed on cloud infrastructure instead of self-hosted servers. 

## Developer productivity tools

### Visualize JSON files

Nested JSON files are hard to read.

**JsonCrack** generates graph diagrams from JSON files and makes them easy to read.

Additionally, the generated diagrams can be downloaded as images.

<p>
  <img src="images/json-cracker.jpeg" />
</p>


### Automatically turn code into architecture diagrams

<p>
  <img src="images/diagrams_as_code.jpeg" style="width: 640px" />
</p>


What does it do?

- Draw the cloud system architecture in Python code.
- Diagrams can also be rendered directly inside the Jupyter Notebooks.
- No design tools are needed. 
- Supports the following providers: AWS, Azure, GCP, Kubernetes, Alibaba Cloud, Oracle Cloud, etc. 
 
[Github repo](https://github.com/mingrammer/diagrams)

## Linux

### Linux file system explained

<p>
  <img src="images/linux-file-systems.jpg" style="width: 680px" />
</p>

The Linux file system used to resemble an unorganized town where individuals constructed their houses wherever they pleased. However, in 1994, the Filesystem Hierarchy Standard (FHS) was introduced to bring order to the Linux file system.

By implementing a standard like the FHS, software can ensure a consistent layout across various Linux distributions. Nonetheless, not all Linux distributions strictly adhere to this standard. They often incorporate their own unique elements or cater to specific requirements.
To become proficient in this standard, you can begin by exploring. Utilize commands such as "cd" for navigation and "ls" for listing directory contents. Imagine the file system as a tree, starting from the root (/). With time, it will become second nature to you, transforming you into a skilled Linux administrator.

### 18 Most-used Linux Commands You Should Know 

Linux commands are instructions for interacting with the operating system. They help manage files, directories, system processes, and many other aspects of the system. You need to become familiar with these commands in order to navigate and maintain Linux-based systems efficiently and effectively. 

This diagram below shows popular Linux commands: 

<p>
  <img src="images/18 Most-Used Linux Commands You Should Know-01.jpeg" style="width: 680px" />
</p>


- ls - List files and directories 
- cd - Change the current directory 
- mkdir - Create a new directory 
- rm - Remove files or directories 
- cp - Copy files or directories 
- mv - Move or rename files or directories 
- chmod - Change file or directory permissions 
- grep - Search for a pattern in files 
- find - Search for files and directories 
- tar - manipulate tarball archive files 
- vi - Edit files using text editors 
- cat - display the content of files 
- top - Display processes and resource usage 
- ps - Display processes information 
- kill - Terminate a process by sending a signal 
- du - Estimate file space usage 
- ifconfig - Configure network interfaces  
- ping - Test network connectivity between hosts 

## Security

### Session, cookie, JWT, token, SSO, and OAuth 2.0 - what are they?

These terms are all related to user identity management. When you log into a website, you declare who you are (identification). Your identity is verified (authentication), and you are granted the necessary permissions (authorization). Many solutions have been proposed in the past, and the list keeps growing.

<p>
  <img src="images/session.jpeg" />
</p>

From simple to complex, here is my understanding of user identity management:

- WWW-Authenticate is the most basic method. You are asked for the username and password by the browser. As a result of the inability to control the login life cycle, it is seldom used today.

- A finer control over the login life cycle is session-cookie. The server maintains session storage, and the browser keeps the ID of the session. A cookie usually only works with browsers and is not mobile app friendly.

- To address the compatibility issue, the token can be used. The client sends the token to the server, and the server validates the token. The downside is that the token needs to be encrypted and decrypted, which may be time-consuming.

- JWT is a standard way of representing tokens. This information can be verified and trusted because it is digitally signed. Since JWT contains the signature, there is no need to save session information on the server side.

- By using SSO (single sign-on), you can sign on only once and log in to multiple websites. It uses CAS (central authentication service) to maintain cross-site information.

- By using OAuth 2.0, you can authorize one website to access your information on another website.



* basic authentication 
  - https://en.wikipedia.org/wiki/Basic_access_authentication
  - https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/WWW-Authenticate
  - HTTP user agent to provide a user name and password; a request contains a header field in the form of Authorization:Basic<credentials>, where credentials is base64 encoded of id:pwd
  - it does not require cookie, session, but use basic HTTP header; 
  - Because the BA field has to be sent in the header of each HTTP request, the web browser needs to cache credentials for a reasonable period of time to avoid constantly prompting the user for their username and password. Caching policy differs between browsers. where the crendential will be cached!!!

* cookie / token vs. JWT (https://devops.com/session-tokens-vs-jwts-choosing-your-session-management-solution/)
  - Token
    - once authenticated, the user’s authentication state is stored in a server-side database as a record that includes 
      - a primary identifier for the session (typically a random string that is at least 128 bits long), 
      - an identifier for the user, 
      - the time the session started, -
      - the expiry of the session and, 
      - sometimes, additional contextual information like the IP address.
    - the session identifier is sent back to the client to be stored as a cookie in the user’s browser.
    - enable more control but introduce some latency (server side token validation).
  - JWT
    - the user’s authentication data is stored as a JSON object, client-side, as soon as it’s issued by the server.
    - no server side latency, but demand more developer investment to address their security complexities and ensure that the right guardrails are in place to prevent vulnerabilities.
  - hybrid
    - return both a session_token and a JWT when a user starts a session
    - session_token is a static value that is good for the lifetime of the session
    - while the JWT has its own, shorter-lived expiry, expired JWTs can be passed to the session API in order to retrieve a fresh JWT, and the servers ensure that the underlying session is still active before passing back a new JWT.

* SSO vs. LDAP (lightweight directory access protocal) (https://en.wikipedia.org/wiki/Single_sign-on)
  - Same sign-on achived by Directory Server Authentication: refers to systems requiring authentication for each application but using the same credentials from a directory server
    - A common use of LDAP is to provide a central place to store usernames and passwords. This allows many different applications and services to connect to the LDAP server to validate users.
    - play an important role in developing intranet and Internet applications by allowing the sharing of information about users, systems, networks, services, and applications throughout the network.
    - As examples, directory services may provide any organized set of records, often with a hierarchical structure, such as a corporate email directory. 
  - SSO refers to systems where a single authentication provides access to multiple applications by passing the authentication token seamlessly to configured applications
    - which component store the authentication token
    - which component will pass authentication token? 
    - simple version of SSO: achieved over IP networks using cookies, sites/services share a common DNS parent domain
    - re-visit to the sso work flow (https://www.onelogin.com/learn/how-single-sign-on-works)
      1. A user browses to the application/service
      2. The Service Provider sends a token that contains some information about the user, like their email address, to the SSO system, aka, the Identity Provider, as part of a request to authenticate the user.
      3. The Identity Provider first checks to see whether the user has already been authenticated
      4. If the user hasn’t logged in, they will be prompted to do so by providing the credentials required by the Identity Provider
      5. it will send a token back to the Service Provider confirming a successful authentication. => This token is passed through the user’s browser to the Service Provider.
      6. ID servier <=> service provider: token generated by ID server, received by service provider through user brower, service provider will check with ID server
      7. user => service provider 
    - cons
      - reduced SSO: to have different level of access
  - single sign off/log out: a single action of signing out terminates access to multiple software systems
  - different application/system support different authetication mechanism, sso must internally store the credentials used for initial authentication and translate them to the credentials required for the different mechanisms
  - pros
    - reduce pwd fatigue and time spent on entering pwd
    - simplify administration contorl
* OAuth2.0, stands for open authentication
  - users to level service1 to access user's data on service2, like amazon, google, fb, msft, twitter
  - Designed specifically to work with Hypertext Transfer Protocol (HTTP)
  - OAuth essentially allows access tokens to be issued by authorization server (owned by SERVICE2) to third-party clients SERVICE1 by an authorization server, with the approval of the resource owner.
  - The third party SERVICE2 then uses the access token to access the protected resources hosted by the resource server



### How to store passwords safely in the database and how to validate a password? 

<p>
  <img src="images/salt.jpg" style="width: 720px" />
</p>

 
**Things NOT to do**

- Storing passwords in plain text is not a good idea because anyone with internal access can see them.

- Storing password hashes directly is not sufficient because it is pruned to precomputation attacks, such as rainbow tables. 

- To mitigate precomputation attacks, we salt the passwords. 

**What is salt?**

According to OWASP guidelines, “a salt is a unique, randomly generated string that is added to each password as part of the hashing process”.
 
**How to store a password and salt?**

1. the hash result is unique to each password.
1. The password can be stored in the database using the following format: hash(password + salt).

**How to validate a password?**

To validate a password, it can go through the following process:

1. A client enters the password.
1. The system fetches the corresponding salt from the database.
1. The system appends the salt to the password and hashes it. Let’s call the hashed value H1.
1. The system compares H1 and H2, where H2 is the hash stored in the database. If they are the same, the password is valid. 

Recap
* It has two tables on application side:
  - user id -> salt
  - user id -> hash(salt + pwd)
* questions
  - if the pwd is seen when transport on internet? use encrypted version
  - server side still see the real pwd but not storing any where (not even logged) or to write only log, or with strongly restricted access


### How does HTTPS work?

Hypertext Transfer Protocol Secure (HTTPS) is an extension of the Hypertext Transfer Protocol (HTTP.) HTTPS transmits encrypted data using Transport Layer Security (TLS.) If the data is hijacked online, all the hijacker gets is binary code. 

<p>
  <img src="images/https.jpg" />
</p>


How is the data encrypted and decrypted?

Step 1 - The client (browser) and the server establish a TCP connection.

Step 2 - The client sends a “client hello” to the server. The message contains a set of necessary encryption algorithms (cipher suites) and the latest TLS version it can support. The server responds with a “server hello” so the browser knows whether it can support the algorithms and TLS version.

The server then sends the SSL certificate to the client. The certificate contains the public key, host name, expiry dates, etc. The client validates the certificate. 

Step 3 - After validating the SSL certificate, the client generates a session key and encrypts it using the public key. The server receives the encrypted session key and decrypts it with the private key. 

Step 4 - Now that both the client and the server hold the same session key (symmetric encryption), the encrypted data is transmitted in a secure bi-directional channel.

Why does HTTPS switch to symmetric encryption during data transmission? There are two main reasons:

1. Security: The asymmetric encryption goes only one way. This means that if the server tries to send the encrypted data back to the client, anyone can decrypt the data using the public key.

2. Server resources: The asymmetric encryption adds quite a lot of mathematical overhead. It is not suitable for data transmissions in long sessions.


How https related to authentication, user|pwd, cookie/token, jwt, sso, auth2.0? 
- this is used in establish secured tcp connection after authenticated
- is the encryption the same as the one during authentication? this SSL, certificates


### Oauth 2.0 Explained With Simple Terms. 

OAuth 2.0 is a powerful and secure framework that allows different applications to securely interact with each other on behalf of users without sharing sensitive credentials. 

<p>
  <img src="images/oAuth2.jpg" />
</p>

The entities involved in OAuth are the User, the Server, and the Identity Provider (IDP). 

What Can an OAuth Token Do? 

When you use OAuth, you get an OAuth token that represents your identity and permissions. This token can do a few important things: 

Single Sign-On (SSO): With an OAuth token, you can log into multiple services or apps using just one login, making life easier and safer. 

Authorization Across Systems: The OAuth token allows you to share your authorization or access rights across various systems, so you don't have to log in separately everywhere. 

Accessing User Profile: Apps with an OAuth token can access certain parts of your user profile that you allow, but they won't see everything. 

Remember, OAuth 2.0 is all about keeping you and your data safe while making your online experiences seamless and hassle-free across different applications and services.

### Top 4 Forms of Authentication Mechanisms 

<p>
  <img src="images/top4-most-used-auth.jpg" />
</p>

1. SSH Keys: 
   
    Cryptographic keys are used to access remote systems and servers securely 

1. OAuth Tokens: 

    Tokens that provide limited access to user data on third-party applications 

1. SSL Certificates: 
  
    Digital certificates ensure secure and encrypted communication between servers and clients 

1. Credentials: 

    User authentication information is used to verify and grant access to various systems and services



### Explaining JSON Web Token (JWT) to a 10 year old Kid

<p>
  <img src="images/jwt.jpg" />
</p>

Imagine you have a special box called a JWT. Inside this box, there are three parts: a header, a payload, and a signature.

The header is like the label on the outside of the box. It tells us what type of box it is and how it's secured. It's usually written in a format called JSON, which is just a way to organize information using curly braces { } and colons : .

The payload is like the actual message or information you want to send. It could be your name, age, or any other data you want to share. It's also written in JSON format, so it's easy to understand and work with.
Now, the signature is what makes the JWT secure. It's like a special seal that only the sender knows how to create. The signature is created using a secret code, kind of like a password. This signature ensures that nobody can tamper with the contents of the JWT without the sender knowing about it.

When you want to send the JWT to a server, you put the header, payload, and signature inside the box. Then you send it over to the server. The server can easily read the header and payload to understand who you are and what you want to do.

### How does Google Authenticator (or other types of 2-factor authenticators) work?

Google Authenticator is commonly used for logging into our accounts when 2-factor authentication is enabled. How does it guarantee security?
 
Google Authenticator is a software-based authenticator that implements a two-step verification service. The diagram below provides detail. 

<p>
  <img src="images/google_authenticate.jpeg" />
</p>


There are two stages involved:

- Stage 1 - The user enables Google two-step verification. 
- Stage 2 - The user uses the authenticator for logging in, etc.

Let’s look at these stages.
 
**Stage 1**

Steps 1 and 2: Bob opens the web page to enable two-step verification. The front end requests a secret key. The authentication service generates the secret key for Bob and stores it in the database.
 
Step 3: The authentication service returns a URI to the front end. The URI is composed of a key issuer, username, and secret key. The URI is displayed in the form of a QR code on the web page.
 
Step 4: Bob then uses Google Authenticator to scan the generated QR code. The secret key is stored in the authenticator.

**Stage 2**
Steps 1 and 2: Bob wants to log into a website with Google two-step verification. For this, he needs the password. Every 30 seconds, Google Authenticator generates a 6-digit password using TOTP (Time-based One Time Password) algorithm. Bob uses the password to enter the website.
 
Steps 3 and 4: The frontend sends the password Bob enters to the backend for authentication. The authentication service reads the secret key from the database and generates a 6-digit password using the same TOTP algorithm as the client.
 
Step 5: The authentication service compares the two passwords generated by the client and the server, and returns the comparison result to the frontend. Bob can proceed with the login process only if the two passwords match.
 
Is this authentication mechanism reasonable and safe? 

- Are the timestamps used by client and server the same? 

    It bascally store key in the user's device => prove if the user has the device
    If user change device, then the key has to be redo?
    If it is based on the initial timestamp when secret key was created 

- Can the secret key be obtained by others? 

    We need to make sure the secret key is transmitted using HTTPS. The authenticator client and the database store the secret key, and we need to make sure the secret keys are encrypted.

- Can the 6-digit password be guessed by hackers?
    
    No. The password has 6 digits, so the generated password has 1 million potential combinations. Plus, the password changes every 30 seconds. If hackers want to guess the password in 30 seconds, they need to enter 30,000 combinations per second.


##  Real World Case Studies

### Netflix's Tech Stack

This post is based on research from many Netflix engineering blogs and open-source projects. If you come across any inaccuracies, please feel free to inform us.

<p>
  <img src="images/netflix tech stack.png" style="width: 680px" />
</p>

**Mobile and web**: Netflix has adopted Swift and Kotlin to build native mobile apps. For its web application, it uses React.

**Frontend/server communication**: Netflix uses GraphQL.

**Backend services**: Netflix relies on ZUUL, Eureka, the Spring Boot framework, and other technologies.

**Databases**: Netflix utilizes EV cache, Cassandra, CockroachDB, and other databases.

**Messaging/streaming**: Netflix employs Apache Kafka and Fink for messaging and streaming purposes.

**Video storage**: Netflix uses S3 and Open Connect for video storage.

**Data processing**: Netflix utilizes Flink and Spark for data processing, which is then visualized using Tableau. Redshift is used for processing structured data warehouse information.

**CI/CD**: Netflix employs various tools such as JIRA, Confluence, PagerDuty, Jenkins, Gradle, Chaos Monkey, Spinnaker, Atlas, and more for CI/CD processes.

### Twitter Architecture 2022

Yes, this is the real Twitter architecture. It is posted by Elon Musk and redrawn by us for better readability. 

<p>
  <img src="images/twitter-arch.jpeg" />
</p>


### Evolution of Airbnb’s microservice architecture over the past 15 years

Airbnb’s microservice architecture went through 3 main stages. 

<p>
  <img src="images/airbnb_arch.jpeg" />
</p>


Monolith (2008 - 2017)

Airbnb began as a simple marketplace for hosts and guests. This is built in a Ruby on Rails application - the monolith. 

What’s the challenge?

- Confusing team ownership + unowned code
- Slow deployment 

Microservices (2017 - 2020)

Microservice aims to solve those challenges. In the microservice architecture, key services include:

- Data fetching service
- Business logic data service
- Write workflow service
- UI aggregation service
- Each service had one owning team

What’s the challenge?

Hundreds of services and dependencies were difficult for humans to manage.

Micro + macroservices (2020 - present)

This is what Airbnb is working on now. The micro and macroservice hybrid model focuses on the unification of APIs.

### Monorepo vs. Microrepo. 

Which is the best? Why do different companies choose different options? 

<p>
  <img src="images/monorepo-microrepo.jpg" />
</p>


Monorepo isn't new; Linux and Windows were both created using Monorepo. To improve scalability and build speed, Google developed its internal dedicated toolchain to scale it faster and strict coding quality standards to keep it consistent. 

Amazon and Netflix are major ambassadors of the Microservice philosophy. This approach naturally separates the service code into separate repositories. It scales faster but can lead to governance pain points later on. 

Within Monorepo, each service is a folder, and every folder has a BUILD config and OWNERS permission control. Every service member is responsible for their own folder. 

On the other hand, in Microrepo, each service is responsible for its repository, with the build config and permissions typically set for the entire repository. 

In Monorepo, dependencies are shared across the entire codebase regardless of your business, so when there's a version upgrade, every codebase upgrades their version. 

In Microrepo, dependencies are controlled within each repository. Businesses choose when to upgrade their versions based on their own schedules. 

Monorepo has a standard for check-ins. Google's code review process is famously known for setting a high bar, ensuring a coherent quality standard for Monorepo, regardless of the business. 

Microrepo can either set its own standard or adopt a shared standard by incorporating the best practices. It can scale faster for business, but the code quality might be a bit different. 
Google engineers built Bazel, and Meta built Buck. There are other open-source tools available, including Nix, Lerna, and others. 

Over the years, Microrepo has had more supported tools, including Maven and Gradle for Java, NPM for NodeJS, and CMake for C/C++, among others. 

### How will you design the Stack Overflow website? 

If your answer is on-premise servers and monolith (on the bottom of the following image), you would likely fail the interview, but that's how it is built in reality!

<p>
  <img src="images/stackoverflow.jpg" />
</p>


**What people think it should look like**

The interviewer is probably expecting something like the top portion of the picture.

- Microservice is used to decompose the system into small components.
- Each service has its own database. Use cache heavily.
- The service is sharded.
- The services talk to each other asynchronously through message queues.
- The service is implemented using Event Sourcing with CQRS.
- Showing off knowledge in distributed systems such as eventual consistency, CAP theorem, etc.

**What it actually is**

Stack Overflow serves all the traffic with only 9 on-premise web servers, and it’s on monolith! It has its own servers and does not run on the cloud.

This is contrary to all our popular beliefs these days. 

### Why did Amazon Prime Video monitoring move from serverless to monolithic? How can it save 90% cost?

The diagram below shows the architecture comparison before and after the migration. 

<p>
  <img src="images/serverless-to-monolithic.jpeg" />
</p>


What is Amazon Prime Video Monitoring Service? 

Prime Video service needs to monitor the quality of thousands of live streams. The monitoring tool automatically analyzes the streams in real time and identifies quality issues like block corruption, video freeze, and sync problems. This is an important process for customer satisfaction. 

There are 3 steps: media converter, defect detector, and real-time notification. 

- What is the problem with the old architecture? 

  The old architecture was based on Amazon Lambda, which was good for building services quickly. However, it was not cost-effective when running the architecture at a high scale. The two most expensive operations are: 

1. The orchestration workflow - AWS step functions charge users by state transitions and the orchestration performs multiple state transitions every second. 

2. Data passing between distributed components - the intermediate data is stored in Amazon S3 so that the next stage can download. The download can be costly when the volume is high. 

- Monolithic architecture saves 90% cost 

  A monolithic architecture is designed to address the cost issues. There are still 3 components, but the media converter and defect detector are deployed in the same process, saving the cost of passing data over the network. Surprisingly, this approach to deployment architecture change led to 90% cost savings! 

This is an interesting and unique case study because microservices have become a go-to and fashionable choice in the tech industry. It's good to see that we are having more discussions about evolving the architecture and having more honest discussions about its pros and cons. Decomposing components into distributed microservices comes with a cost. 

- What did Amazon leaders say about this? 
  
  Amazon CTO Werner Vogels: “Building **evolvable software systems** is a strategy, not a religion. And revisiting your architecture with an open mind is a must.” 

Ex Amazon VP Sustainability Adrian Cockcroft: “The Prime Video team had followed a path I call **Serverless First**…I don’t advocate **Serverless Only**”. 

### How does Disney Hotstar capture 5 Billion Emojis during a tournament?

<p>
  <img src="images/hotstar_emojis.jpeg" style="width: 720px" />
</p>


1. Clients send emojis through standard HTTP requests. You can think of Golang Service as a typical Web Server. Golang is chosen because it supports concurrency well. Threads in Golang are lightweight.

2. Since the write volume is very high, Kafka (message queue) is used as a buffer.

3. Emoji data are aggregated by a streaming processing service called Spark. It aggregates data every 2 seconds, which is configurable. There is a trade-off to be made based on the interval. A shorter interval means emojis are delivered to other clients faster but it also means more computing resources are needed.

4. Aggregated data is written to another Kafka. 

5. The PubSub consumers pull aggregated emoji data from Kafka. 

6. Emojis are delivered to other clients in real-time through the PubSub infrastructure. The PubSub infrastructure is interesting. Hotstar considered the following protocols: Socketio, NATS, MQTT, and gRPC, and settled with MQTT.
 
A similar design is adopted by LinkedIn which streams a million likes/sec.

### How Discord Stores Trillions Of Messages 

The diagram below shows the evolution of message storage at Discord: 

<p>
  <img src="images/discord-store-messages.jpg" />
</p>


MongoDB ➡️ Cassandra ➡️ ScyllaDB 

In 2015, the first version of Discord was built on top of a single MongoDB replica. Around Nov 2015, MongoDB stored 100 million messages and the RAM couldn’t hold the data and index any longer. The latency became unpredictable. Message storage needs to be moved to another database. Cassandra was chosen. 

In 2017, Discord had 12 Cassandra nodes and stored billions of messages. 

At the beginning of 2022, it had 177 nodes with trillions of messages. At this point, latency was unpredictable, and maintenance operations became too expensive to run. 

There are several reasons for the issue: 

- Cassandra uses the LSM tree for the internal data structure. The reads are more expensive than the writes. There can be many concurrent reads on a server with hundreds of users, resulting in hotspots. 
- Maintaining clusters, such as compacting SSTables, impacts performance. 
- Garbage collection pauses would cause significant latency spikes 

ScyllaDB is Cassandra compatible database written in C++. Discord redesigned its architecture to have a monolithic API, a data service written in Rust, and ScyllaDB-based storage. 

The p99 read latency in ScyllaDB is 15ms compared to 40-125ms in Cassandra. The p99 write latency is 5ms compared to 5-70ms in Cassandra. 

### How do video live streamings work on YouTube, TikTok live, or Twitch?
 
Live streaming differs from regular streaming because the video content is sent via the internet in real-time, usually with a latency of just a few seconds.
 
The diagram below explains what happens behind the scenes to make this possible.

<p>
  <img src="images/live_streaming_updated.jpg" style="width: 640px" />
</p>

 
Step 1: The raw video data is captured by a microphone and camera. The data is sent to the server side.
 
Step 2: The video data is compressed and encoded. For example, the compressing algorithm separates the background and other video elements. After compression, the video is encoded to standards such as H.264. The size of the video data is much smaller after this step.
 
Step 3: The encoded data is divided into smaller segments, usually seconds in length, so it takes much less time to download or stream.
 
Step 4: The segmented data is sent to the streaming server. The streaming server needs to support different devices and network conditions. This is called ‘Adaptive Bitrate Streaming.’ This means we need to produce multiple files at different bitrates in steps 2 and 3.
 
Step 5: The live streaming data is pushed to edge servers supported by CDN (Content Delivery Network.) Millions of viewers can watch the video from an edge server nearby. CDN significantly lowers data transmission latency. 
 
Step 6: The viewers’ devices decode and decompress the video data and play the video in a video player.
 
Steps 7 and 8: If the video needs to be stored for replay, the encoded data is sent to a storage server, and viewers can request a replay from it later.
 
Standard protocols for live streaming include:

- RTMP (Real-Time Messaging Protocol): This was originally developed by Macromedia to transmit data between a Flash player and a server. Now it is used for streaming video data over the internet. Note that video conferencing applications like Skype use RTC (Real-Time Communication) protocol for lower latency.
- HLS (HTTP Live Streaming): It requires the H.264 or H.265 encoding. Apple devices accept only HLS format.
- DASH (Dynamic Adaptive Streaming over HTTP): DASH does not support Apple devices.
- Both HLS and DASH support adaptive bitrate streaming.

## License

<p xmlns:cc="http://creativecommons.org/ns#" >This work is licensed under <a href="http://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC-ND 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nd.svg?ref=chooser-v1"></a></p>
