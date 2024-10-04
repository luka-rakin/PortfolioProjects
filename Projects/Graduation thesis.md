# Platform for Education and Distribution of Teaching Materials with Limited Access

[View the Repository Here](https://github.com/orgs/Diplomski-rad/repositories)

## Project Overview

This project, developed as my final thesis, is a Platform for Education and Distribution of Teaching Materials with Limited Access. It serves as a platform for sharing and selling educational video content, or courses, across a wide range of skills, from cooking and fitness to software development and beyond. The focus of the project was on protecting video content from unauthorized sharing and distribution, as well as implementing a secure payment system.

## Key Features

- **Video Course Marketplace**: Users can browse, purchase, and access various educational video courses.

- **Two User Roles:**

  - **Standard User**: Can view publicly available courses, purchase them, and access the purchased course content for educational purposes.
  - **Author:** Users who wish to share their knowledge can create and manage their own courses, upload videos, and earn revenue from course sales.

- **Content Protection:** The platform emphasizes video content protection, though full protection was not achieved with free versions of the video hosting services. However, with paid versions, such as the Pro version of the Dailymotion API, full content protection could be implemented.

- **Secure Payments:** The PayPal API was integrated to ensure secure transactions between users and the platform for course purchases.

## Technology Stack

### Backend

- **ASP.NET**

  - The backend was developed using **ASP.NET**, following a layered architecture where each layer is responsible for its specialized logic (Controller, Service, Repository). This promotes cleaner code and easier maintainability.
  - **Entity Framework Core** was used as an Object-Relational Mapper (ORM) to handle database interactions, providing an efficient and flexible way to query and manage data.
  - The application uses **PostgreSQL** as the database for storing user data, course details, transactions, and other essential information.
  - **Dependency Injection** was used to decouple components, making the system more modular and extendable.

### Frontend

- **React:**

  - The frontend was developed using React, leveraging reusable components to ensure consistent interface elements.
  - **React Router** was used to enable smooth navigation between different parts of the application.

### APIs Integrated

- **Dailymotion API:**

  - Used for hosting and streaming video content. The free version was used during development, but it is important to note that the paid version would meet all the platform's content protection requirements.

- **PayPal API:**
  - Integrated for handling secure payments, ensuring users can safely purchase courses on the platform.

## Challenges and Solutions

Due to the time constraints and complexity of building video hosting, a custom video player, and a payment system, I decided to integrate Dailymotion and PayPal, which are well-established solutions. While the free version of Dailymotion did not allow full content protection, the platform is built with the capability to upgrade to the paid version, which would provide the necessary security features.

## Project Motivation

As this was my final thesis project, I aimed to incorporate all the knowledge and skills I gained throughout my studies, applying them in a real-world scenario. The project was developed entirely by myself, covering both the frontend and backend aspects.

## Repository Structure

- **Frontend:** Contains the React codebase, including reusable components and routing.
- **Backend:** Contains the ASP.NET solution with layered architecture and dependency injection implemented.
