# projects-to-make
Major Projects Portfolio

This repository includes two major software engineering projects that I plan to build as part of my journey toward becoming a well-rounded software engineer.

The projects cover several important areas of modern software development, including backend engineering, distributed systems, cloud computing, full-stack development, and application deployment.

Rather than focusing only on theory, I want to use these projects to gain hands-on experience designing, building, testing, and deploying real-world applications using technologies commonly found in the industry.

Project 1: Distributed Real-Time Financial Data Pipeline

Proposed Timeline: Month 6
Project Domain: FinTech | Distributed Systems | Backend Engineering | Cloud Computing

1. Project Overview

The Distributed Real-Time Financial Data Pipeline is a cloud-based project focused on collecting, processing, and storing simulated financial market data in real time.

The idea behind this project is to understand how financial platforms handle large streams of incoming data while keeping processing fast, reliable, and scalable.

The system will generate simulated market events, such as stock price changes, trading volumes, and transactions. These events will be sent through Apache Kafka, processed by independent backend services, and stored in a database for later analysis.

Through this project, I want to explore how different services communicate, how real-time data pipelines work, and how distributed applications handle continuous data streams.

2. Project Objectives
Understand distributed systems and microservices architecture.
Build real-time data processing capabilities.
Learn event-driven architecture using Apache Kafka.
Implement communication between independent backend services.
Work with databases and caching systems.
Gain practical experience with Docker and cloud infrastructure.
Set up automated testing and CI/CD workflows.
3. Technology Stack
Technology	Purpose
Go	Building high-performance data processing services
Python	Financial data simulation and processing utilities
Apache Kafka	Real-time event streaming and messaging
PostgreSQL	Storing processed financial data
Redis	Caching frequently accessed data
Docker	Containerizing application services
AWS EC2	Cloud hosting and deployment
GitHub Actions	Automated testing and CI/CD
4. System Architecture

The application will use an event-driven microservices architecture, where individual services handle different parts of the data pipeline.

Data Flow:

Data Generator: A Python application will generate simulated financial market data, including stock prices, timestamps, and trading volumes.
Kafka Producer: Publishes generated events to Kafka topics.
Kafka Broker: Manages communication and distributes events between producers and consumers.
Data Processing Service: A Go-based service will consume incoming events, validate the data, and perform the necessary transformations.
Redis Cache: Stores frequently accessed market information for faster retrieval.
PostgreSQL Database: Stores processed financial records for persistent storage and future analysis.
Monitoring and Testing: Tracks processing performance, application errors, and service reliability.
5. Implementation Plan
Phase 1: Project Setup
Set up the development environment.
Create and organize the project repository.
Configure Docker and Docker Compose.
Set up PostgreSQL, Redis, and Apache Kafka.
Phase 2: Financial Data Simulation
Build a Python-based financial data generator.
Generate simulated stock prices and trading events.
Define a structured JSON format for financial events.
Implement a Kafka producer to publish generated data.
Phase 3: Real-Time Data Processing
Develop a Go-based Kafka consumer.
Implement event validation and data transformation.
Process incoming financial events.
Handle invalid messages and processing failures.
Phase 4: Database and Caching Integration
Integrate PostgreSQL for persistent data storage.
Use Redis to cache frequently accessed information.
Improve database queries and data retrieval performance.
Phase 5: Testing and Performance Evaluation
Write unit and integration tests.
Measure event processing latency.
Evaluate throughput under different workloads.
Test service reliability and error-handling mechanisms.
Phase 6: Cloud Deployment and Automation
Deploy the application on AWS EC2.
Containerize application services using Docker.
Configure GitHub Actions for automated testing.
Set up a basic CI/CD pipeline.
6. Expected Features
Real-time ingestion of simulated financial market data.
Event-driven communication using Apache Kafka.
Distributed data processing through independent services.
Faster data retrieval using Redis caching.
Persistent data storage with PostgreSQL.
Docker-based service deployment.
Automated testing and deployment workflows.
Basic performance and latency monitoring.
7. Expected Outcome

By the end of this project, I want to have a much better understanding of how distributed backend systems and real-time data pipelines work in practice.

The completed application should demonstrate how to build an event-driven system that can continuously ingest, process, and store financial data while maintaining reliable communication between independent services.

Key Learning Outcomes:

Distributed systems fundamentals.
Event-driven microservices architecture.
Real-time data streaming and processing.
Backend development using Go and Python.
Database optimization and caching.
Docker-based application deployment.
AWS cloud infrastructure.
CI/CD and automated testing.
Project 2: Cloud-Native Collaborative Task Management System

Proposed Timeline: Month 9
Project Domain: Full-Stack Development | Cloud Computing | Web Applications | Software Engineering

1. Project Overview

The Cloud-Native Collaborative Task Management System will be a web application that allows individuals and teams to organize projects, assign tasks, manage deadlines, and track progress from one place.

The application will include a responsive dashboard where users can manage their tasks, collaborate with team members, and stay updated on project activities. It will also support real-time updates so that changes made by one user are reflected for other connected users.

My main goal with this project is to build a complete full-stack application while getting practical experience with frontend development, backend APIs, database management, authentication, authorization, and cloud deployment.

I also want to understand how different parts of a modern web application work together, from the user interface to the backend services and cloud infrastructure.

2. Project Objectives
Build a modern and responsive frontend application.
Develop RESTful APIs using Node.js and Express.
Learn database design and integration with MongoDB.
Implement secure user authentication and authorization.
Set up role-based access control (RBAC).
Enable real-time communication using WebSockets.
Explore cloud storage and content delivery.
Implement basic application monitoring and deployment.
3. Technology Stack
Technology	Purpose
React	Building the frontend user interface
TypeScript	Type-safe application development
Node.js	Backend runtime environment
Express.js	Developing RESTful APIs
MongoDB	Storing users, tasks, and project data
WebSockets	Real-time updates and communication
Docker	Application containerization
AWS S3	Cloud-based file storage
AWS CloudFront	Content delivery and distribution
GitHub Actions	Automated testing and CI/CD
4. Core Application Modules
A. User Authentication

This module will handle user registration, login, and access to protected parts of the application.

Planned functionality:

User registration and login.
Secure password hashing.
Token-based authentication.
Protected application routes.
User session management.
B. Task Management

The task management module will allow users to create, organize, assign, and track tasks.

Planned functionality:

Create, update, and delete tasks.
Assign tasks to team members.
Set task priorities and deadlines.
Track task status.
Filter and search tasks.
C. Collaborative Dashboard

The dashboard will provide an overview of ongoing projects and individual responsibilities.

Planned functionality:

Display assigned tasks.
Show overall project progress.
View pending and completed tasks.
Organize tasks by project.
Provide a responsive and easy-to-use interface.
D. Role-Based Access Control (RBAC)

Different users will have different levels of access depending on their roles.

Role	Permissions
Admin	Manage users, projects, and permissions
Manager	Create projects and assign tasks
Member	View and update assigned tasks
E. Real-Time Communication

WebSockets will be used to keep users updated without requiring them to manually refresh the application.

Planned functionality:

Real-time task updates.
Notifications when tasks are assigned.
Broadcast task status changes.
Synchronize updates across connected users.
F. Cloud Storage and Monitoring

This module will handle file storage, content delivery, and basic application monitoring.

Planned functionality:

Upload and store files using AWS S3.
Deliver static frontend assets through CloudFront.
Monitor application health and server performance.
Track application errors and basic activity.
5. Implementation Plan
Phase 1: Frontend Development
Set up React and TypeScript.
Design the overall application layout.
Build reusable UI components.
Develop responsive dashboard pages.
Implement frontend routing.
Phase 2: Backend Development
Configure Node.js and Express.
Design RESTful API endpoints.
Build user and task management APIs.
Integrate MongoDB.
Implement data validation and error handling.
Phase 3: Authentication and Authorization
Develop user registration and login functionality.
Implement secure password hashing.
Configure token-based authentication.
Create protected API routes.
Implement role-based access control.
Phase 4: Real-Time Collaboration
Integrate WebSockets.
Implement real-time task updates.
Build notification functionality.
Synchronize updates between connected users.
Phase 5: Cloud Integration
Configure AWS S3 for file storage.
Set up AWS CloudFront for content delivery.
Containerize the application using Docker.
Prepare the production environment.
Phase 6: Testing and Deployment
Write frontend and backend tests.
Test REST APIs and authentication.
Perform integration testing.
Configure GitHub Actions.
Deploy the application.
Set up basic monitoring and logging.
6. Expected Features
Secure user registration and login.
Responsive collaborative dashboard.
Task creation, assignment, and tracking.
Project and team management.
Role-based access control.
Real-time task updates using WebSockets.
File uploads through AWS S3.
Cloud-based frontend delivery using CloudFront.
Docker-based application deployment.
Automated testing and CI/CD.
Basic application monitoring.
7. Expected Outcome

By completing this project, I want to gain hands-on experience building a complete full-stack application and taking it from development to cloud deployment.

The finished application should bring together a modern frontend, a structured backend, database integration, secure authentication, and real-time collaboration.

It will also give me an opportunity to understand how cloud services are used to store files, deliver application assets, and support a deployed web application.

Key Learning Outcomes:

Full-stack application development.
React and TypeScript.
RESTful API development.
Node.js and Express backend architecture.
MongoDB database integration.
Authentication and authorization.
Role-based access control.
Real-time communication using WebSockets.
AWS cloud services.
Docker and CI/CD workflows.
Overall Project Timeline
Timeline	Project	Primary Focus
Month 6	Distributed Real-Time Financial Data Pipeline	Distributed systems and real-time data processing
Month 9	Cloud-Native Collaborative Task Management System	Full-stack development and cloud deployment
Overall Learning Goals

Both projects are intended to help me move beyond basic programming exercises and develop a deeper understanding of how modern software applications are designed, built, and deployed.

Throughout this process, I want to focus on the following areas:

Backend Engineering: Building reliable APIs, handling application logic, and developing scalable backend services.
Distributed Systems: Understanding event-driven architecture, message brokers, service communication, and distributed processing.
Full-Stack Development: Building complete applications using modern frontend and backend technologies.
Database Engineering: Working with relational and NoSQL databases, caching systems, and efficient data management.
Cloud Computing: Learning how to deploy, configure, and manage applications using AWS services.
DevOps: Getting practical experience with Docker, CI/CD pipelines, automated testing, and deployment workflows.
System Design: Understanding how scalability, performance, reliability, and architectural decisions affect real-world applications.
Final Goal

My goal is to complete both projects with working implementations, clean and maintainable code, proper documentation, automated tests, and cloud deployment.

I don't just want these projects to be collections of technologies or features. I want them to demonstrate that I can take an idea, plan its architecture, develop the application, test its functionality, and deploy it in a practical environment.

Together, these projects will help me build a strong foundation in backend engineering, distributed systems, full-stack development, and cloud-native technologies. They will also serve as practical portfolio projects that showcase my technical growth and ability to work with modern software engineering tools.

Note: Both projects are currently planned implementations. Their features, architecture, performance benchmarks, and deployment details will be updated as development progresses.
