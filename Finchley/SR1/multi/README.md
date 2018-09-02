Spring Cloud

#1. Features
##I. Cloud Native Applications
###2. Spring Cloud Context: Application Context Services
####2.1. The Bootstrap Application Context
####2.2. Application Context Hierarchies
####2.3. Changing the Location of Bootstrap Properties
####2.4. Overriding the Values of Remote Properties
####2.5. Customizing the Bootstrap Configuration
####2.6. Customizing the Bootstrap Property Sources
####2.7. Logging Configuration
####2.8. Environment Changes
####2.9. Refresh Scope
####2.10. Encryption and Decryption
####2.11. Endpoints
###3. Spring Cloud Commons: Common Abstractions
####3.1. @EnableDiscoveryClient
#####3.1.1. Health Indicator
####3.2. ServiceRegistry
#####3.2.1. ServiceRegistry Auto-Registration
#####3.2.2. Service Registry Actuator Endpoint
####3.3. Spring RestTemplate as a Load Balancer Client
####3.4. Spring WebClient as a Load Balancer Client
#####3.4.1. Retrying Failed Requests
####3.5. Multiple RestTemplate objects
####3.6. Spring WebFlux WebClient as a Load Balancer Client
####3.7. Ignore Network Interfaces
####3.8. HTTP Client Factories
####3.9. Enabled Features
#####3.9.1. Feature types
#####3.9.2. Declaring features
##II. Spring Cloud Config
###4. Quick Start
####4.1. Client Side Usage
###5. Spring Cloud Config Server
####5.1. Environment Repository
#####5.1.1. Git Backend
######Skipping SSL Certificate Validation
######Setting HTTP Connection Timeout
######Placeholders in Git URI
######Pattern Matching and Multiple Repositories
######Authentication
######Authentication with AWS CodeCommit
######Git SSH configuration using properties
######Placeholders in Git Search Paths
######Force pull in Git Repositories
######Deleting untracked branches in Git Repositories
#####5.1.2. Version Control Backend Filesystem Use
#####5.1.3. File System Backend
#####5.1.4. Vault Backend
######Multiple Properties Sources
#####5.1.5. Accessing Backends Through a Proxy
#####5.1.6. Sharing Configuration With All Applications
######File Based Repositories
######Vault Server
#####5.1.7. JDBC Backend
#####5.1.8. Composite Environment Repositories
######Custom Composite Environment Repositories
#####5.1.9. Property Overrides
####5.2. Health Indicator
####5.3. Security
####5.4. Encryption and Decryption
####5.5. Key Management
####5.6. Creating a Key Store for Testing
####5.7. Using Multiple Keys and Key Rotation
####5.8. Serving Encrypted Properties
###6. Serving Alternative Formats
###7. Serving Plain Text
###8. Embedding the Config Server
###9. Push Notifications and Spring Cloud Bus
###10. Spring Cloud Config Client
####10.1. Config First Bootstrap
####10.2. Discovery First Bootstrap
####10.3. Config Client Fail Fast
####10.4. Config Client Retry
####10.5. Locating Remote Configuration Resources
####10.6. Specifying Multiple Urls for the Config Server
####10.7. Configuring Read Timeouts
####10.8. Security
#####10.8.1. Health Indicator
#####10.8.2. Providing A Custom RestTemplate
#####10.8.3. Vault
####10.9. Nested Keys In Vault
##III. Spring Cloud Netflix
###11. Service Discovery: Eureka Clients
####11.1. How to Include Eureka Client
####11.2. Registering with Eureka
####11.3. Authenticating with the Eureka Server
####11.4. Status Page and Health Indicator
####11.5. Registering a Secure Application
####11.6. Eureka’s Health Checks
####11.7. Eureka Metadata for Instances and Clients
#####11.7.1. Using Eureka on Cloud Foundry
#####11.7.2. Using Eureka on AWS
#####11.7.3. Changing the Eureka Instance ID
####11.8. Using the EurekaClient
#####11.8.1. EurekaClient without Jersey
####11.9. Alternatives to the Native Netflix EurekaClient
####11.10. Why Is It so Slow to Register a Service?
####11.11. Zones
###12. Service Discovery: Eureka Server
####12.1. How to Include Eureka Server
####12.2. How to Run a Eureka Server
####12.3. High Availability, Zones and Regions
####12.4. Standalone Mode
####12.5. Peer Awareness
####12.6. When to Prefer IP Address
####12.7. Securing The Eureka Server
###13. Circuit Breaker: Hystrix Clients
####13.1. How to Include Hystrix
####13.2. Propagating the Security Context or Using Spring Scopes
####13.3. Health Indicator
####13.4. Hystrix Metrics Stream
###14. Circuit Breaker: Hystrix Dashboard
###15. Hystrix Timeouts And Ribbon Clients
####15.1. How to Include the Hystrix Dashboard
####15.2. Turbine
#####15.2.1. Clusters Endpoint
####15.3. Turbine Stream
###16. Client Side Load Balancer: Ribbon
####16.1. How to Include Ribbon
####16.2. Customizing the Ribbon Client
####16.3. Customizing the Default for All Ribbon Clients
####16.4. Customizing the Ribbon Client by Setting Properties
####16.5. Using Ribbon with Eureka
####16.6. Example: How to Use Ribbon Without Eureka
####16.7. Example: Disable Eureka Use in Ribbon
####16.8. Using the Ribbon API Directly
####16.9. Caching of Ribbon Configuration
####16.10. How to Configure Hystrix Thread Pools
####16.11. How to Provide a Key to Ribbon’s IRule
###17. External Configuration: Archaius
###18. Router and Filter: Zuul
####18.1. How to Include Zuul
####18.2. Embedded Zuul Reverse Proxy
####18.3. Zuul Http Client
####18.4. Cookies and Sensitive Headers
####18.5. Ignored Headers
####18.6. Management Endpoints
#####18.6.1. Routes Endpoint
#####18.6.2. Filters Endpoint
####18.7. Strangulation Patterns and Local Forwards
####18.8. Uploading Files through Zuul
####18.9. Query String Encoding
####18.10. Plain Embedded Zuul
####18.11. Disable Zuul Filters
####18.12. Providing Hystrix Fallbacks For Routes
####18.13. Zuul Timeouts
####18.14. Rewriting the Location header
####18.15. Metrics
####18.16. Zuul Developer Guide
#####18.16.1. The Zuul Servlet
#####18.16.2. Zuul RequestContext
#####18.16.3. @EnableZuulProxy vs. @EnableZuulServer
#####18.16.4. @EnableZuulServer Filters
#####18.16.5. @EnableZuulProxy Filters
#####18.16.6. Custom Zuul Filter Examples
######How to Write a Pre Filter
######How to Write a Route Filter
######How to Write a Post Filter
#####18.16.7. How Zuul Errors Work
#####18.16.8. Zuul Eager Application Context Loading
###19. Polyglot support with Sidecar
###20. Retrying Failed Requests
####20.1. BackOff Policies
####20.2. Configuration
#####20.2.1. Zuul
###21. HTTP Clients
IV. Spring Cloud OpenFeign
22. Declarative REST Client: Feign
22.1. How to Include Feign
22.2. Overriding Feign Defaults
22.3. Creating Feign Clients Manually
22.4. Feign Hystrix Support
22.5. Feign Hystrix Fallbacks
22.6. Feign and @Primary
22.7. Feign Inheritance Support
22.8. Feign request/response compression
22.9. Feign logging
V. Spring Cloud Stream
23. Quick Start
23.1. Creating a Sample Application by Using Spring Initializr
23.2. Importing the Project into Your IDE
23.3. Adding a Message Handler, Building, and Running
24. What’s New in 2.0?
24.1. New Features and Components
24.2. Notable Enhancements
24.2.1. Both Actuator and Web Dependencies Are Now Optional
24.2.2. Content-type Negotiation Improvements
24.3. Notable Deprecations
24.3.1. Java Serialization (Java Native and Kryo)
24.3.2. Deprecated Classes and Methods
25. Introducing Spring Cloud Stream
26. Main Concepts
26.1. Application Model
26.1.1. Fat JAR
26.2. The Binder Abstraction
26.3. Persistent Publish-Subscribe Support
26.4. Consumer Groups
26.5. Consumer Types
26.5.1. Durability
26.6. Partitioning Support
27. Programming Model
27.1. Destination Binders
27.2. Destination Bindings
27.3. Producing and Consuming Messages
27.3.1. Spring Integration Support
27.3.2. Using @StreamListener Annotation
27.3.3. Using @StreamListener for Content-based routing
27.3.4. Using Polled Consumers
27.4. Error Handling
27.4.1. Application Error Handling
27.4.2. System Error Handling
Drop Failed Messages
DLQ - Dead Letter Queue
Re-queue Failed Messages
27.4.3. Retry Template
27.5. Reactive Programming Support
27.5.1. Reactor-based Handlers
27.5.2. Reactive Sources
28. Binders
28.1. Producers and Consumers
28.2. Binder SPI
28.3. Binder Detection
28.3.1. Classpath Detection
28.4. Multiple Binders on the Classpath
28.5. Connecting to Multiple Systems
28.6. Binding visualization and control
28.7. Binder Configuration Properties
29. Configuration Options
29.1. Binding Service Properties
29.2. Binding Properties
29.2.1. Common Binding Properties
29.2.2. Consumer Properties
29.2.3. Producer Properties
29.3. Using Dynamically Bound Destinations
30. Content Type Negotiation
30.1. Mechanics
30.1.1. Content Type versus Argument Type
30.1.2. Message Converters
30.2. Provided MessageConverters
30.3. User-defined Message Converters
31. Schema Evolution Support
31.1. Schema Registry Client
31.1.1. Schema Registry Client Properties
31.2. Avro Schema Registry Client Message Converters
31.2.1. Avro Schema Registry Message Converter Properties
31.3. Apache Avro Message Converters
31.4. Converters with Schema Support
31.5. Schema Registry Server
31.5.1. Schema Registry Server API
Registering a New Schema
Retrieving an Existing Schema by Subject, Format, and Version
Retrieving an Existing Schema by Subject and Format
Retrieving an Existing Schema by ID
Deleting a Schema by Subject, Format, and Version
Deleting a Schema by ID
Deleting a Schema by Subject
31.5.2. Using Confluent’s Schema Registry
31.6. Schema Registration and Resolution
31.6.1. Schema Registration Process (Serialization)
31.6.2. Schema Resolution Process (Deserialization)
32. Inter-Application Communication
32.1. Connecting Multiple Application Instances
32.2. Instance Index and Instance Count
32.3. Partitioning
32.3.1. Configuring Output Bindings for Partitioning
32.3.2. Configuring Input Bindings for Partitioning
33. Testing
33.1. Disabling the Test Binder Autoconfiguration
34. Health Indicator
35. Metrics Emitter
36. Samples
36.1. Deploying Stream Applications on CloudFoundry
VI. Binder Implementations
37. Apache Kafka Binder
37.1. Usage
37.2. Apache Kafka Binder Overview
37.3. Configuration Options
37.3.1. Kafka Binder Properties
37.3.2. Kafka Consumer Properties
37.3.3. Kafka Producer Properties
37.3.4. Usage examples
Example: Setting autoCommitOffset to false and Relying on Manual Acking
Example: Security Configuration
Example: Pausing and Resuming the Consumer
37.4. Error Channels
37.5. Kafka Metrics
37.6. Dead-Letter Topic Processing
37.7. Partitioning with the Kafka Binder
38. Apache Kafka Streams Binder
38.1. Usage
38.2. Kafka Streams Binder Overview
38.2.1. Streams DSL
38.3. Configuration Options
38.3.1. Kafka Streams Properties
38.3.2. TimeWindow properties:
38.4. Multiple Input Bindings
38.4.1. Multiple Input Bindings as a Sink
38.4.2. Multiple Input Bindings as a Processor
38.5. Multiple Output Bindings (aka Branching)
38.6. Message Conversion
38.6.1. Outbound serialization
38.6.2. Inbound Deserialization
38.7. Error Handling
38.7.1. Handling Deserialization Exceptions
38.7.2. Handling Non-Deserialization Exceptions
38.8. Interactive Queries
38.9. Accessing the underlying KafkaStreams object
39. RabbitMQ Binder
39.1. Usage
39.2. RabbitMQ Binder Overview
39.3. Configuration Options
39.3.1. RabbitMQ Binder Properties
39.3.2. RabbitMQ Consumer Properties
39.3.3. Rabbit Producer Properties
39.4. Retry With the RabbitMQ Binder
39.4.1. Putting it All Together
39.5. Error Channels
39.6. Dead-Letter Queue Processing
39.6.1. Non-Partitioned Destinations
39.6.2. Partitioned Destinations
republishToDlq=false
republishToDlq=true
39.7. Partitioning with the RabbitMQ Binder
VII. Spring Cloud Bus
40. Quick Start
41. Bus Endpoints
41.1. Bus Refresh Endpoint
41.2. Bus Env Endpoint
42. Addressing an Instance
43. Addressing All Instances of a Service
44. Service ID Must Be Unique
45. Customizing the Message Broker
46. Tracing Bus Events
47. Broadcasting Your Own Events
47.1. Registering events in custom packages
VIII. Spring Cloud Sleuth
48. Introduction
48.1. Terminology
48.2. Purpose
48.2.1. Distributed Tracing with Zipkin
48.2.2. Visualizing errors
48.2.3. Distributed Tracing with Brave
48.2.4. Live examples
48.2.5. Log correlation
JSON Logback with Logstash
48.2.6. Propagating Span Context
Baggage versus Span Tags
48.3. Adding Sleuth to the Project
48.3.1. Only Sleuth (log correlation)
48.3.2. Sleuth with Zipkin via HTTP
48.3.3. Sleuth with Zipkin over RabbitMQ or Kafka
49. Additional Resources
50. Features
50.1. Introduction to Brave
50.1.1. Tracing
50.1.2. Local Tracing
50.1.3. Customizing Spans
50.1.4. Implicitly Looking up the Current Span
50.1.5. RPC tracing
One-Way tracing
51. Sampling
51.1. Declarative sampling
51.2. Custom sampling
51.3. Sampling in Spring Cloud Sleuth
52. Propagation
52.1. Propagating extra fields
52.1.1. Prefixed fields
52.1.2. Extracting a Propagated Context
52.1.3. Sharing span IDs between Client and Server
52.1.4. Implementing Propagation
53. Current Tracing Component
54. Current Span
54.1. Setting a span in scope manually
55. Instrumentation
56. Span lifecycle
56.1. Creating and finishing spans
56.2. Continuing Spans
56.3. Creating a Span with an explicit Parent
57. Naming spans
57.1. @SpanName Annotation
57.2. toString() method
58. Managing Spans with Annotations
58.1. Rationale
58.2. Creating New Spans
58.3. Continuing Spans
58.4. Advanced Tag Setting
58.4.1. Custom extractor
58.4.2. Resolving Expressions for a Value
58.4.3. Using the toString() method
59. Customizations
59.1. HTTP
59.2. TracingFilter
59.3. Custom service name
59.4. Customization of Reported Spans
59.5. Host Locator
60. Sending Spans to Zipkin
61. Zipkin Stream Span Consumer
62. Integrations
62.1. OpenTracing
62.2. Runnable and Callable
62.3. Hystrix
62.3.1. Custom Concurrency Strategy
62.3.2. Manual Command setting
62.4. RxJava
62.5. HTTP integration
62.5.1. HTTP Filter
62.5.2. HandlerInterceptor
62.5.3. Async Servlet support
62.5.4. WebFlux support
62.5.5. Dubbo RPC support
62.6. HTTP Client Integration
62.6.1. Synchronous Rest Template
62.6.2. Asynchronous Rest Template
Multiple Asynchronous Rest Templates
62.6.3. WebClient
62.6.4. Traverson
62.6.5. Apache HttpClientBuilder and HttpAsyncClientBuilder
62.6.6. Netty HttpClient
62.6.7. UserInfoRestTemplateCustomizer
62.7. Feign
62.8. Asynchronous Communication
62.8.1. @Async Annotated methods
62.8.2. @Scheduled Annotated Methods
62.8.3. Executor, ExecutorService, and ScheduledExecutorService
Customization of Executors
62.9. Messaging
62.9.1. Spring Integration and Spring Cloud Stream
62.9.2. Spring RabbitMq
62.9.3. Spring Kafka
62.10. Zuul
63. Running examples
IX. Spring Cloud Consul
64. Install Consul
65. Consul Agent
66. Service Discovery with Consul
66.1. How to activate
66.2. Registering with Consul
66.3. HTTP Health Check
66.3.1. Metadata and Consul tags
66.3.2. Making the Consul Instance ID Unique
66.4. Looking up services
66.4.1. Using Ribbon
66.4.2. Using the DiscoveryClient
66.5. Consul Catalog Watch
67. Distributed Configuration with Consul
67.1. How to activate
67.2. Customizing
67.3. Config Watch
67.4. YAML or Properties with Config
67.5. git2consul with Config
67.6. Fail Fast
68. Consul Retry
69. Spring Cloud Bus with Consul
69.1. How to activate
70. Circuit Breaker with Hystrix
71. Hystrix metrics aggregation with Turbine and Consul
X. Spring Cloud Zookeeper
72. Install Zookeeper
73. Service Discovery with Zookeeper
73.1. Activating
73.2. Registering with Zookeeper
73.3. Using the DiscoveryClient
74. Using Spring Cloud Zookeeper with Spring Cloud Netflix Components
74.1. Ribbon with Zookeeper
75. Spring Cloud Zookeeper and Service Registry
75.1. Instance Status
76. Zookeeper Dependencies
76.1. Using the Zookeeper Dependencies
76.2. Activating Zookeeper Dependencies
76.3. Setting up Zookeeper Dependencies
76.3.1. Aliases
76.3.2. Path
76.3.3. Load Balancer Type
76.3.4. Content-Type Template and Version
76.3.5. Default Headers
76.3.6. Required Dependencies
76.3.7. Stubs
76.4. Configuring Spring Cloud Zookeeper Dependencies
77. Spring Cloud Zookeeper Dependency Watcher
77.1. Activating
77.2. Registering a Listener
77.3. Using the Presence Checker
78. Distributed Configuration with Zookeeper
78.1. Activating
78.2. Customizing
78.3. Access Control Lists (ACLs)
XI. Spring Boot Cloud CLI
79. Installation
80. Running Spring Cloud Services in Development
80.1. Adding Additional Applications
81. Writing Groovy Scripts and Running Applications
82. Encryption and Decryption
XII. Spring Cloud Security
83. Quickstart
83.1. OAuth2 Single Sign On
83.2. OAuth2 Protected Resource
84. More Detail
84.1. Single Sign On
84.2. Token Relay
84.2.1. Client Token Relay
84.2.2. Client Token Relay in Zuul Proxy
84.2.3. Resource Server Token Relay
85. Configuring Authentication Downstream of a Zuul Proxy
XIII. Spring Cloud for Cloud Foundry
86. Discovery
87. Single Sign On
XIV. Spring Cloud Contract
88. Spring Cloud Contract
89. Spring Cloud Contract Verifier Introduction
89.1. Why a Contract Verifier?
89.1.1. Testing issues
89.2. Purposes
89.3. How It Works
89.3.1. A Three-second Tour
On the Producer Side
On the Consumer Side
89.3.2. A Three-minute Tour
On the Producer Side
On the Consumer Side
89.3.3. Defining the Contract
89.3.4. Client Side
89.3.5. Server Side
89.4. Step-by-step Guide to Consumer Driven Contracts (CDC)
89.4.1. Technical note
89.4.2. Consumer side (Loan Issuance)
89.4.3. Producer side (Fraud Detection server)
89.4.4. Consumer Side (Loan Issuance) Final Step
89.5. Dependencies
89.6. Additional Links
89.6.1. Spring Cloud Contract video
89.6.2. Readings
89.7. Samples
90. Spring Cloud Contract FAQ
90.1. Why use Spring Cloud Contract Verifier and not X ?
90.2. I don’t want to write a contract in Groovy!
90.3. What is this value(consumer(), producer()) ?
90.4. How to do Stubs versioning?
90.4.1. API Versioning
90.4.2. JAR versioning
90.4.3. Dev or prod stubs
90.5. Common repo with contracts
90.5.1. Repo structure
90.5.2. Workflow
90.5.3. Consumer
90.5.4. Producer
90.5.5. How can I define messaging contracts per topic not per producer?
For Maven Project
For Gradle Project
90.6. Do I need a Binary Storage? Can’t I use Git?
90.6.1. Protocol convention
90.6.2. Producer
90.6.3. Consumer
90.7. Can I use the Pact Broker?
90.7.1. Pact Consumer
90.7.2. Producer
90.7.3. Pact Consumer (Producer Contract approach)
90.8. How can I debug the request/response being sent by the generated tests client?
90.8.1. How can I debug the mapping/request/response being sent by WireMock?
90.8.2. How can I see what got registered in the HTTP server stub?
90.8.3. Can I reference text from file?
91. Spring Cloud Contract Verifier Setup
91.1. Gradle Project
91.1.1. Prerequisites
91.1.2. Add Gradle Plugin with Dependencies
91.1.3. Gradle and Rest Assured 2.0
91.1.4. Snapshot Versions for Gradle
91.1.5. Add stubs
91.1.6. Run the Plugin
91.1.7. Default Setup
91.1.8. Configure Plugin
91.1.9. Configuration Options
91.1.10. Single Base Class for All Tests
91.1.11. Different Base Classes for Contracts
91.1.12. Invoking Generated Tests
91.1.13. Pushing stubs to SCM
91.1.14. Spring Cloud Contract Verifier on the Consumer Side
91.2. Maven Project
91.2.1. Add maven plugin
91.2.2. Maven and Rest Assured 2.0
91.2.3. Snapshot versions for Maven
91.2.4. Add stubs
91.2.5. Run plugin
91.2.6. Configure plugin
91.2.7. Configuration Options
91.2.8. Single Base Class for All Tests
91.2.9. Different base classes for contracts
91.2.10. Invoking generated tests
91.2.11. Pushing stubs to SCM
91.2.12. Maven Plugin and STS
91.3. Stubs and Transitive Dependencies
91.4. CI Server setup
91.5. Scenarios
91.6. Docker Project
91.6.1. Short intro to Maven, JARs and Binary storage
91.6.2. How it works
Environment Variables
91.6.3. Example of usage
91.6.4. Server side (nodejs)
92. Spring Cloud Contract Verifier Messaging
92.1. Integrations
92.2. Manual Integration Testing
92.3. Publisher-Side Test Generation
92.3.1. Scenario 1: No Input Message
92.3.2. Scenario 2: Output Triggered by Input
92.3.3. Scenario 3: No Output Message
92.4. Consumer Stub Generation
93. Spring Cloud Contract Stub Runner
93.1. Snapshot versions
93.2. Publishing Stubs as JARs
93.3. Stub Runner Core
93.3.1. Retrieving stubs
Stub downloading
Classpath scanning
93.3.2. Running stubs
Limitations
Running using main app
HTTP Stubs
Viewing registered mappings
Messaging Stubs
93.4. Stub Runner JUnit Rule
93.4.1. Maven settings
93.4.2. Providing fixed ports
93.4.3. Fluent API
93.4.4. Stub Runner with Spring
93.5. Stub Runner Spring Cloud
93.5.1. Stubbing Service Discovery
Test profiles and service discovery
93.5.2. Additional Configuration
93.6. Stub Runner Boot Application
93.6.1. How to use it?
Stub Runner Server
Stub Runner Server Fat Jar
Spring Cloud CLI
93.6.2. Endpoints
HTTP
Messaging
93.6.3. Example
93.6.4. Stub Runner Boot with Service Discovery
93.7. Stubs Per Consumer
93.8. Common
93.8.1. Common Properties for JUnit and Spring
93.8.2. Stub Runner Stubs IDs
93.9. Stub Runner Docker
93.9.1. How to use it
93.9.2. Example of client side usage in a non JVM project
94. Stub Runner for Messaging
94.1. Stub triggering
94.1.1. Trigger by Label
94.1.2. Trigger by Group and Artifact Ids
94.1.3. Trigger by Artifact Ids
94.1.4. Trigger All Messages
94.2. Stub Runner Integration
94.2.1. Adding the Runner to the Project
94.2.2. Disabling the functionality
Scenario 1 (no input message)
Scenario 2 (output triggered by input)
Scenario 3 (input with no output)
94.3. Stub Runner Stream
94.3.1. Adding the Runner to the Project
94.3.2. Disabling the functionality
Scenario 1 (no input message)
Scenario 2 (output triggered by input)
Scenario 3 (input with no output)
94.4. Stub Runner Spring AMQP
94.4.1. Adding the Runner to the Project
Triggering the message
Spring AMQP Test Configuration
95. Contract DSL
95.1. Limitations
95.2. Common Top-Level elements
95.2.1. Description
95.2.2. Name
95.2.3. Ignoring Contracts
95.2.4. Passing Values from Files
95.2.5. HTTP Top-Level Elements
95.3. Request
95.4. Response
95.5. Dynamic properties
95.5.1. Dynamic properties inside the body
95.5.2. Regular expressions
95.5.3. Passing Optional Parameters
95.5.4. Executing Custom Methods on the Server Side
95.5.5. Referencing the Request from the Response
95.5.6. Registering Your Own WireMock Extension
95.5.7. Dynamic Properties in the Matchers Sections
95.6. JAX-RS Support
95.7. Async Support
95.8. Working with Context Paths
95.9. Working with Web Flux
95.10. Messaging Top-Level Elements
95.10.1. Output Triggered by a Method
95.10.2. Output Triggered by a Message
95.10.3. Consumer/Producer
95.10.4. Common
95.11. Multiple Contracts in One File
95.12. Generating Spring REST Docs snippets from the contracts
96. Customization
96.1. Extending the DSL
96.1.1. Common JAR
96.1.2. Adding the Dependency to the Project
96.1.3. Test the Dependency in the Project’s Dependencies
96.1.4. Test a Dependency in the Plugin’s Dependencies
96.1.5. Referencing classes in DSLs
97. Using the Pluggable Architecture
97.1. Custom Contract Converter
97.1.1. Pact Converter
97.1.2. Pact Contract
97.1.3. Pact for Producers
97.1.4. Pact for Consumers
97.2. Using the Custom Test Generator
97.3. Using the Custom Stub Generator
97.4. Using the Custom Stub Runner
97.5. Using the Custom Stub Downloader
97.6. Using the SCM Stub Downloader
97.7. Using the Pact Stub Downloader
98. Spring Cloud Contract WireMock
98.1. Registering Stubs Automatically
98.2. Using Files to Specify the Stub Bodies
98.3. Alternative: Using JUnit Rules
98.4. Relaxed SSL Validation for Rest Template
98.5. WireMock and Spring MVC Mocks
98.6. Customization of WireMock configuration
98.7. Generating Stubs using REST Docs
98.8. Generating Contracts by Using REST Docs
99. Migrations
99.1. 1.0.x → 1.1.x
99.1.1. New structure of generated stubs
99.2. 1.1.x → 1.2.x
99.2.1. Custom HttpServerStub
99.2.2. New packages for generated tests
99.2.3. New Methods in TemplateProcessor
99.2.4. RestAssured 3.0
99.3. 1.2.x → 2.0.x
99.3.1. No Camel support
100. Links
XV. Spring Cloud Vault
101. Quick Start
102. Client Side Usage
102.1. Authentication
103. Authentication methods
103.1. Token authentication
103.2. AppId authentication
103.2.1. Custom UserId
103.3. AppRole authentication
103.4. AWS-EC2 authentication
103.5. AWS-IAM authentication
103.6. TLS certificate authentication
103.7. Cubbyhole authentication
103.8. Kubernetes authentication
104. Secret Backends
104.1. Generic Backend
104.2. Versioned Key-Value Backend
104.3. Consul
104.4. RabbitMQ
104.5. AWS
105. Database backends
105.1. Database
105.2. Apache Cassandra
105.3. MongoDB
105.4. MySQL
105.5. PostgreSQL
106. Configure PropertySourceLocator behavior
107. Service Registry Configuration
108. Vault Client Fail Fast
109. Vault Client SSL configuration
110. Lease lifecycle management (renewal and revocation)
XVI. Spring Cloud Gateway
111. How to Include Spring Cloud Gateway
112. Glossary
113. How It Works
114. Route Predicate Factories
114.1. After Route Predicate Factory
114.2. Before Route Predicate Factory
114.3. Between Route Predicate Factory
114.4. Cookie Route Predicate Factory
114.5. Header Route Predicate Factory
114.6. Host Route Predicate Factory
114.7. Method Route Predicate Factory
114.8. Path Route Predicate Factory
114.9. Query Route Predicate Factory
114.10. RemoteAddr Route Predicate Factory
114.10.1. Modifying the way remote addresses are resolved
115. GatewayFilter Factories
115.1. AddRequestHeader GatewayFilter Factory
115.2. AddRequestParameter GatewayFilter Factory
115.3. AddResponseHeader GatewayFilter Factory
115.4. Hystrix GatewayFilter Factory
115.5. PrefixPath GatewayFilter Factory
115.6. PreserveHostHeader GatewayFilter Factory
115.7. RequestRateLimiter GatewayFilter Factory
115.7.1. Redis RateLimiter
115.8. RedirectTo GatewayFilter Factory
115.9. RemoveNonProxyHeaders GatewayFilter Factory
115.10. RemoveRequestHeader GatewayFilter Factory
115.11. RemoveResponseHeader GatewayFilter Factory
115.12. RewritePath GatewayFilter Factory
115.13. SaveSession GatewayFilter Factory
115.14. SecureHeaders GatewayFilter Factory
115.15. SetPath GatewayFilter Factory
115.16. SetResponseHeader GatewayFilter Factory
115.17. SetStatus GatewayFilter Factory
115.18. StripPrefix GatewayFilter Factory
115.19. Retry GatewayFilter Factory
116. Global Filters
116.1. Combined Global Filter and GatewayFilter Ordering
116.2. Forward Routing Filter
116.3. LoadBalancerClient Filter
116.4. Netty Routing Filter
116.5. Netty Write Response Filter
116.6. RouteToRequestUrl Filter
116.7. Websocket Routing Filter
116.8. Gateway Metrics Filter
116.9. Making An Exchange As Routed
117. TLS / SSL
118. Configuration
118.1. Fluent Java Routes API
118.2. DiscoveryClient Route Definition Locator
119. CORS Configuration
120. Actuator API
121. Developer Guide
121.1. Writing Custom Route Predicate Factories
121.2. Writing Custom GatewayFilter Factories
121.3. Writing Custom Global Filters
121.4. Writing Custom Route Locators and Writers
122. Building a Simple Gateway Using Spring MVC or Webflux
XVII. Spring Cloud Function
123. Introduction
124. Getting Started
125. Building and Running a Function
126. Function Catalog and Flexible Function Signatures
127. Standalone Web Applications
128. Standalone Streaming Applications
129. Deploying a Packaged Function
130. Dynamic Compilation
131. Serverless Platform Adapters
131.1. AWS Lambda
131.1.1. Introduction
131.1.2. Notes on JAR Layout
131.1.3. Upload
131.1.4. Platfom Specific Features
HTTP and API Gateway
131.2. Azure Functions
131.2.1. Notes on JAR Layout
131.2.2. JSON Configuration
131.2.3. Build
131.2.4. Running the sample
131.3. Apache Openwhisk
131.3.1. Quick Start
XVIII. Appendix: Compendium of Configuration Properties