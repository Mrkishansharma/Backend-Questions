# Node.js and Web Development FAQ

This repository contains a list of frequently asked questions and their answers related to Node.js and web development concepts.

## Table of Contents
1. [Blocking vs Non-Blocking](#blocking-vs-non-blocking)
2. [Throughput](#throughput)
3. [Difference between readFile and readFileSync](#difference-between-readfile-and-readfilesync)
4. [Making a network request using http module](#making-a-network-request-using-http-module)
5. [Creating a web server without express](#creating-a-web-server-without-express)
6. [Understanding libuv](#libuv)
7. [Phases involved in the event loop](#phases-involved-in-the-event-loop)
8. [Timers in Node.js](#timers-in-nodejs)
9. [Node Version Manager (NVM)](#node-version-manager)
10. [Common.js vs ES modules](#commonjs-vs-es-modules)
11. [Working of the crypto module](#crypto-module)
12. [Websockets](#websockets)
13. [Microservices](#microservices)
14. [Creating a CLI based app using Node.js and publishing it](#creating-a-cli-based-app)
15. [How Express works](#how-express-works)
16. [Routes in Express](#routes-in-express)
17. [Middlewares in Express](#middlewares-in-express)
18. [MVC framework](#mvc-framework)
19. [Validations in Node.js](#validations-in-nodejs)
20. [Static routing in Node.js](#static-routing-in-nodejs)
21. [Templating engines](#templating-engines)
22. [Session management in Express](#session-management-in-express)
23. [Cookie management with Express](#cookie-management-with-express)
24. [Common libraries for Express](#common-libraries-for-express)
25. [Cross-Origin Resource Sharing (CORS)](#cors)
26. [Testing in Node.js](#testing-in-nodejs)
27. [Unit testing](#unit-testing)
28. [Functional testing](#functional-testing)
29. [HTTP vs HTTPS](#http-vs-https)
30. [SSL/TLS](#ssltls)
31. [OWASP](#owasp)
32. [SQL vs NoSQL databases](#sql-vs-nosql-databases)
33. [Common SQL queries](#common-sql-queries)
34. [Joins in SQL](#joins-in-sql)
35. [Lookup in MongoDB](#lookup-in-mongodb)
36. [CAP theorem](#cap-theorem)
37. [Indexing](#indexing)
38. [Database replication](#database-replication)
39. [PACELC](#pacelc)
40. [Normalization and Denormalization](#normalization-and-denormalization)
41. [Entity Relationship Model (ER Model)](#entity-relationship-model-er-model)

## Blocking vs Non-Blocking
- **Overview**: Blocking code execution blocks further execution until the current operation is completed, while non-blocking code allows other operations to run concurrently without waiting for the current one to finish.

## Throughput
- **Overview**: Throughput refers to the rate at which a system can process tasks or transfer data, typically measured in requests per second (RPS) or bits per second (bps).

## Difference between readFile and readFileSync
- **Overview**: The `readFile` function in Node.js reads a file asynchronously, meaning it won't block other operations, while `readFileSync` reads the file synchronously, blocking the execution until the file is read.

## Making a network request using http module
- **Overview**: To make a network request in Node.js, you can use the built-in `http` module. It provides functions to create HTTP or HTTPS clients and servers. Refer to the official Node.js documentation for more details: [Anatomy of an HTTP Transaction](https://nodejs.org/en/docs/guides/anatomy-of-an-http-transaction/).

## Creating a web server without express
- **Overview**: You can create a basic web server in Node.js without using Express by utilizing the `http` module to handle incoming HTTP requests and sending responses accordingly.

## Understanding libuv
- **Overview**: libuv is a multi-platform support library used by Node.js to handle asynchronous I/O operations. It abstracts the underlying operating system functionalities for networking, file system, and more.

## Phases involved in the event loop
- **Overview**: The Node.js event loop has multiple phases, including timers, pending callbacks, idle, poll, check, close callbacks, and process.nextTick. These phases handle different types of asynchronous operations.

## Timers in Node.js
- **Overview**: Node.js provides functions like `setTimeout` and `setInterval` to schedule operations for a specific time interval or delay.

## Node Version Manager (NVM)
- **Overview**: NVM is a tool that allows you to manage multiple Node.js versions on your system and switch between them easily.

## Common.js vs ES modules
- **Overview**: Common.js and ES modules are two different formats for organizing and importing modules in Node.js. Common.js uses `require` and `module.exports`, while ES modules use `import` and `export`.

## Working of the crypto module
- **Overview**: The crypto module in Node.js provides cryptographic functionalities, such as encryption, decryption, hashing, and more.

## Websockets
- **Overview**: Websockets enable real-time bidirectional communication between clients and servers, allowing server-initiated updates to client applications.

## Microservices
- **Overview**: Microservices is an architectural approach where an application is divided into smaller, loosely coupled services, each responsible for specific functionalities.

## Creating a CLI based app using Node.js and publishing it
- **Overview**: You can build a Command-Line Interface (CLI) based application using Node.js, and publish it to platforms like npm for easy distribution.

## How Express works
- **Overview**: Express is a popular Node.js web application framework that simplifies the development of web applications by providing a set of robust features and tools.

## Routes in Express
- **Overview**: In Express, routes define how the application responds to different HTTP requests and URLs.

## Middlewares in Express
- **Overview**: Middlewares in Express are functions that have access to the request and response objects and can modify them, perform additional operations, or invoke the next middleware in the stack.

## MVC framework
- **Overview**: The Model-View-Controller (MVC) is a design pattern commonly used in web development to separate the application into three interconnected components: Model, View, and Controller.

## Validations in Node.js
- **Overview**: Validations in Node.js are performed to ensure that the input data meets certain criteria or constraints before processing.

## Static routing in Node.js
- **Overview**: Static routing in Node.js involves serving static files (e.g., HTML, CSS, JS) directly to the client without any processing.

## Templating engines
- **Overview**: Templating engines in Node.js allow you to generate dynamic HTML by embedding variables or logic into the markup.

## Session management in Express
- **Overview**: Session management in Express involves creating and maintaining user sessions to keep track of user-specific data between multiple requests.

## Cookie management with Express
- **Overview**: Cookies in Express are used to store small pieces of data on the client-side, helping to maintain user state and track user interactions.

## Common libraries for Express
- **Overview**: Several libraries can be used alongside Express to extend its functionality, such as Passport.js for authentication and Morgan for logging.

## Cross-Origin Resource Sharing (CORS)
- **Overview**: CORS is a security feature implemented in web browsers to prevent unauthorized access to resources hosted on different domains.

## Testing in Node.js
- **Overview**: Testing in Node.js involves the use of various testing frameworks and methodologies to ensure the reliability and correctness of the code.

## Unit testing
- **Overview**: Unit testing is a type of testing where individual units or components of a software application are tested in isolation to verify their functionality.

## Functional testing
- **Overview**: Functional testing is a type of testing that focuses on testing the application's features and functionality from an end-user perspective.

## HTTP vs HTTPS
- **Overview**: HTTP (Hypertext Transfer Protocol) and HTTPS (Hypertext Transfer Protocol Secure) are two protocols used for communication over the internet. HTTPS is a secure version of HTTP that uses SSL/TLS for encrypted communication.

## SSL/TLS
- **Overview**: SSL (Secure Sockets Layer) and TLS (Transport Layer Security) are cryptographic protocols that provide secure communication over a computer network.

## OWASP
- **Overview**: OWASP (Open Web Application Security Project) is an open-source community focused on improving the security of web applications and software.

## SQL vs NoSQL databases
- **Overview**: SQL (Structured Query Language) databases are relational databases, while NoSQL databases are non-relational databases that use various data models.

## Common SQL queries
- **Overview**: Some common SQL queries include SELECT, INSERT, UPDATE, DELETE, and JOIN, used to interact with relational databases.

## Joins in SQL
- **Overview**: Joins in SQL combine data from two or more database tables based on a related column.

## Lookup in MongoDB
- **Overview**: In MongoDB, the `$lookup` operator is used to perform a left outer join between collections.

## CAP theorem
- **Overview**: The CAP theorem states that in a distributed data system, it is impossible to achieve Consistency, Availability, and Partition tolerance simultaneously.

## Indexing
- **Overview**: Indexing in databases is the process of creating data structures to improve the speed of data retrieval operations.

## Database replication
- **Overview**: Database replication involves copying and maintaining the same data on multiple database servers for redundancy and fault tolerance.

## PACELC
- **Overview**: PACELC theorem describes the trade-offs in distributed systems during network partitions.

## Normalization and Denormalization
- **Overview**: Normalization is the process of organizing data in a database to reduce redundancy, while denormalization combines normalized data for improved query performance.

## Entity Relationship Model (ER Model)
- **Overview**: The Entity Relationship Model is a conceptual data model used to represent the relationships between entities (tables) in a database.

---
