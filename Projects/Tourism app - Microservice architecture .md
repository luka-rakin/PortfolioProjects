# Tourism App - Microservice Architecture

This project was developed as part of the **Service-Oriented Architectures** course, where the goal was to transition the **Tourism App - Modular Monolith** to a microservice architecture using the **Strangler Pattern**. The objective was to progressively migrate each module of the monolithic system into individual microservices, culminating in a fully functional microservice-based architecture.
The project was developed by a team of 4 members

## Technologies Used

- **GO** (Programming Language for Microservices)
- **gRPC** (Communication between Microservices)
- **Docker** (Containerization)
- **API Gateway**
- **Relational Databases, NoSQL, and Graph Databases** (depending on microservice requirements)

## Project Overview

The main purpose of this project was to gain insights into transitioning from a monolithic architecture to microservices, ensuring that each microservice could operate independently while maintaining communication through **gRPC**. The project focused on breaking the monolithic application down module by module, using the strangler pattern, and implementing microservices in Go.

Although we managed to complete most of the project, some parts of the system, particularly in the `docker-compose.yml` file, were commented out due to complications with integrating certain services towards the end. However, this project provided invaluable experience with handling complex migrations, utilizing containers, and working with a diverse range of databases.

## gRPC and Proto Files

**gRPC** was used as the communication protocol between microservices. We learned how to write _proto_ files, defining services and messages within them, which are crucial for gRPC communication. These _proto_ files define the service endpoints and the message structure used between services, and they are then compiled to generate Go code that handles the gRPC calls.

A typical proto file contains:

- **Service Definitions:** Describing the methods that microservices can invoke on each other.
- **Message Definitions:** Specifying the structure of the data being sent and received.

This approach allows us to clearly define the API contracts between microservices, ensuring type safety and efficient communication.

## Docker Setup

**Docker** was used to containerize each microservice and manage them using Docker Compose. By using containers, we ensured that each microservice was isolated, and we could easily deploy and scale them independently.

While Docker Compose made it easier to manage dependencies between services, some parts of the final implementation are commented out due to unresolved issues during deployment ([docker-compose.yml](docker-compose.yml))

## Database Separation

As part of the transition to microservices, we also decoupled the databases used by each service:

- **Relational Databases** were used for certain services that required structured, transactional data.
- **NoSQL Databases** were employed for services needing more flexibility and scalability.
- **Graph Databases** were used for services where relationships between data entities were critical.

## Repository Access

Unfortunately, I am unable to provide access to the entire backend repository as it was forked from the Tourism App - Modular Monolith project, which is private. However, I am able to share a link to the repository containing the microservices that were created during the project. [View the Repository Here](https://github.com/SOA-tim-1)
