# Web Development and System Design FAQ

## Table of Contents
1. [Models](#models)
2. [Mongoose and Promises](#mongoose-and-promises)
3. [Aggregation Pipelines with Mongoose](#aggregation-pipelines-with-mongoose)
4. [Arrow Functions and "this" in Mongoose](#arrow-functions-and-this-in-mongoose)
5. [Connection Management with Mongoose](#connection-management-with-mongoose)
6. [Duplicate Executions in Mongoose](#duplicate-executions-in-mongoose)
7. [Creating Indexes with Mongoose](#creating-indexes-with-mongoose)
8. [Pre and Post Hooks](#pre-and-post-hooks)
9. [Authentication](#authentication)
10. [Authorization](#authorization)
11. [Role-Based Authentication](#role-based-authentication)
12. [Hashing](#hashing)
13. [Encryption](#encryption)
14. [Difference between Hashing and Encryption](#difference-between-hashing-and-encryption)
15. [Salt](#salt)
16. [JWT (JSON Web Tokens)](#jwt-json-web-tokens)
17. [Managing Authentication](#managing-authentication)
18. [Cookie-Based Authentication](#cookie-based-authentication)
19. [Session Management](#session-management)
20. [OAuth](#oauth)
21. [REST API](#rest-api)
22. [gRPC](#grpc)
23. [GraphQL](#graphql)
24. [HTTP](#http)
25. [Web Sockets](#web-sockets)
26. [Caching](#caching)
27. [Backend Caching Methods](#backend-caching-methods)
28. [LRU Cache](#lru-cache)
29. [Redis and its Usage](#redis-and-its-usage)
30. [Frontend Caching Implementation](#frontend-caching-implementation)
31. [Content Delivery Network (CDN)](#content-delivery-network-cdn)
32. [Domain Name System (DNS)](#domain-name-system-dns)
33. [How the Internet Works](#how-the-internet-works)
34. [Browser Functionality](#browser-functionality)
35. [Stateless Backend](#stateless-backend)
36. [Client-Server Model](#client-server-model)
37. [HTTP vs HTTPS](#http-vs-https)
38. [Throughput](#throughput)
39. [Availability](#availability)
40. [Latency](#latency)
41. [Rate Limiting](#rate-limiting)
42. [Rate Limiting Techniques](#rate-limiting-techniques)
43. [Load Balancer](#load-balancer)
44. [Designing an API](#designing-an-api)
45. [Horizontal and Vertical Scaling](#horizontal-and-vertical-scaling)
46. [Building a Reliable System](#building-a-reliable-system)

## Models
- **Overview**: Models in web development refer to the representation of data and the business logic associated with it.

## Mongoose and Promises
- **Overview**: Mongoose, a MongoDB library for Node.js, does not return Promises directly but provides a `.then` method to handle asynchronous operations.

## Aggregation Pipelines with Mongoose
- **Overview**: Aggregation pipelines in Mongoose allow complex data aggregation and transformation operations on MongoDB collections.

## Arrow Functions and "this" in Mongoose
- **Overview**: When using arrow functions for virtuals, middleware, getters/setters, or methods in Mongoose, the value of "this" can be incorrect due to the lexical scoping behavior of arrow functions.

## Connection Management with Mongoose
- **Overview**: Decide whether to create/destroy a new connection for each database operation in Mongoose based on your application's needs and performance considerations.

## Duplicate Executions in Mongoose
- **Overview**: If your query/update seems to execute twice in Mongoose, it might be due to multiple event listeners or callbacks triggering the operation.

## Creating Indexes with Mongoose
- **Overview**: Mongoose allows you to create indexes to improve the query performance of your MongoDB collections.

## Pre and Post Hooks
- **Overview**: Mongoose supports pre and post hooks that allow you to add middleware functions before and after specific operations, like saving or removing a document.

## Authentication
- **Overview**: Authentication is the process of verifying the identity of a user or system.

## Authorization
- **Overview**: Authorization is the process of granting access to specific resources or functionalities to authenticated users.

## Role-Based Authentication
- **Overview**: Role-Based Authentication involves assigning different roles to users based on their permissions and granting access accordingly.

## Hashing
- **Overview**: Hashing is a one-way process of converting data into a fixed-length string, commonly used for storing passwords securely.

## Encryption
- **Overview**: Encryption is the process of converting data into a ciphertext, which can be decrypted back to its original form using a key.

## Difference between Hashing and Encryption
- **Overview**: Hashing and encryption are both cryptographic techniques, but they serve different purposes and have distinct properties.

## Salt
- **Overview**: Salt is random data added to hashed passwords to increase their security against attacks like rainbow tables.

## JWT (JSON Web Tokens)
- **Overview**: JSON Web Tokens (JWT) are a compact and self-contained way to represent information between two parties.

## Managing Authentication
- **Overview**: Explore different ways to manage authentication, such as token-based authentication or session-based authentication.

## Cookie-Based Authentication
- **Overview**: Cookie-Based Authentication involves storing authentication information in cookies to maintain user sessions.

## Session Management
- **Overview**: Session Management refers to the process of maintaining user-specific data between multiple requests.

## OAuth
- **Overview**: OAuth is an open standard for access delegation, allowing applications to access user data from another application without sharing passwords.

## REST API
- **Overview**: REST (Representational State Transfer) is an architectural style for designing networked applications.

## gRPC
- **Overview**: gRPC is an open-source remote procedure call (RPC) framework, designed for high-performance and cross-platform applications.

## GraphQL
- **Overview**: GraphQL is a query language and runtime for APIs, allowing clients to request only the data they need.

## HTTP
- **Overview**: HTTP (Hypertext Transfer Protocol) is the foundation of data communication on the World Wide Web.

## Web Sockets
- **Overview**: Web Sockets enable real-time bidirectional communication between clients and servers.

## Caching
- **Overview**: Caching is the process of storing frequently accessed data in a cache for faster retrieval.

## Backend Caching Methods
- **Overview**: Explore different methods to implement caching on the backend for improving performance.

## LRU Cache
- **Overview**: LRU (Least Recently Used) Cache is a caching mechanism where the least recently accessed items are removed when the cache reaches its limit.

## Redis and its Usage
- **Overview**: Redis is an in-memory data structure store that can be used as a cache, message broker, or database.

## Frontend Caching Implementation
- **Overview**: Learn how to implement caching on the frontend using techniques like browser caching and Service Workers.

## Content Delivery Network (CDN)
- **Overview**: A CDN is a geographically distributed network of servers that delivers web content to users based on their location, improving performance and reliability.

## Domain Name System (DNS)
- **Overview**: DNS is a system that translates human-readable domain names into IP addresses used by computers to locate resources on the internet.

## How the Internet Works
- **Overview**: Understand the fundamental principles of how data is transmitted and exchanged across the internet.

## Browser Functionality
- **Overview**: Explore how web browsers work and how they render and display web pages.

## Stateless Backend
- **Overview**: A stateless backend does not store any client-specific data and treats each request as independent.

## Client-Server Model
- **Overview**: The client-server model is a distributed application structure where clients request resources or services from servers.

## HTTP vs HTTPS
- **Overview**: Compare HTTP and HTTPS protocols, where HTTPS adds an extra layer of security using SSL/TLS.

## Throughput
- **Overview**: Throughput refers to the rate at which a system can process tasks or transfer data.

## Availability
- **Overview**: Availability is a measure of how accessible and operational a system or service is.

## Latency
- **Overview**: Latency is the time delay between initiating a request and receiving a response.

## Rate Limiting
- **Overview**: Rate Limiting restricts the number of requests a client can make within a given time frame to prevent abuse or overloading of a server.

## Rate Limiting Techniques
- **Overview**: Explore various techniques to implement rate limits, such as Token Bucket and Rolling Window.

## Load Balancer
- **Overview**: A load balancer distributes incoming network traffic across multiple servers to ensure optimal resource utilization and prevent overloading.

## Designing an API
- **Overview**: Learn the best practices and considerations for designing a well-structured and scalable API.

## Horizontal and Vertical Scaling
- **Overview**: Horizontal scaling involves adding more machines to distribute the load, while vertical scaling involves increasing the resources on a single machine.

## Building a Reliable System
- **Overview**: Understand the principles and best practices for building a reliable and fault-tolerant system.

---
