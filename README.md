# Online Quiz System

## Project Overview

The **Online Quiz System** is a web-based application designed to
automate the complete online quiz process. The system provides a
centralized platform for students, administrators, and instructors to
manage and participate in quizzes.

The proposed system uses a **microservices-oriented architecture** in
which major functionalities such as authentication, user management,
quiz management, question management, evaluation, and result generation
are separated into independent services. REST APIs are used for
communication between application components.

## Problem Statement

Traditional quiz systems rely on manual question paper preparation,
distribution, evaluation, and result generation, making the overall
process time-consuming and prone to errors. Managing users, questions,
quizzes, and results through separate manual processes is also difficult
and inefficient.

The Online Quiz System addresses these limitations by providing a
centralized and automated platform that can conduct quizzes,
automatically evaluate submitted answers, and generate results quickly.

## Objectives

-   To develop a user-friendly web-based Online Quiz System that enables
    secure student participation and allows administrators/instructors
    to manage quizzes, users, questions, and results.
-   To provide an effective quiz platform with multiple-choice
    questions, correct answers, marks, and time limits.
-   To automatically evaluate submitted answers and quickly generate and
    display quiz scores and results.
-   To implement a microservices-oriented architecture to improve
    scalability, flexibility, and maintainability.

## Key Features

-   User registration and login
-   Secure user authentication
-   Quiz creation and management
-   Question management
-   Multiple-choice questions
-   Marks and time-limit support
-   Online quiz participation
-   Answer submission
-   Automatic answer evaluation
-   Score calculation
-   Result generation and display
-   Centralized management of users, quizzes, questions, answers, and
    results
-   REST API-based communication

## System Architecture

The project follows a web-based, microservices-oriented architecture.

``` text
                    +----------------------+
                    |        Users         |
                    |  Student / Admin     |
                    +----------+-----------+
                               |
                               v
                    +----------------------+
                    |      Frontend        |
                    |   Web Interface      |
                    +----------+-----------+
                               |
                           REST APIs
                               |
                               v
                    +----------------------+
                    |       Backend        |
                    +----------+-----------+
                               |
        +----------+-----------+-----------+----------+----------+
        |          |                       |          |          |
        v          v                       v          v          v
 +----------+ +----------+          +----------+ +----------+ +----------+
 |   Auth   | |   User   |          |   Quiz   | | Question | |Evaluation|
 | Service  | | Service  |          | Service  | | Service  | | Service  |
 +----------+ +----------+          +----------+ +----------+ +----------+
                                                                  |
                                                                  v
                                                          +---------------+
                                                          | Result Service|
                                                          +-------+-------+
                                                                  |
                                                                  v
                                                          +---------------+
                                                          |   Database    |
                                                          +---------------+
```

## Major Components

  Service / Component      Main Function
  ------------------------ --------------------------------------------------------
  Authentication Service   Login and authentication
  User Service             User management
  Quiz Service             Quiz management
  Question Service         Question management
  Evaluation Service       Answer evaluation
  Result Service           Result generation
  Database                 Stores users, quizzes, questions, answers, and results
  REST APIs                Communication between application components

## System Workflow

``` text
User Login
    |
    v
Authentication
    |
    v
Select / Manage Quiz
    |
    v
Retrieve Questions
    |
    v
Attempt Quiz
    |
    v
Submit Answers
    |
    v
Automatic Evaluation
    |
    v
Calculate Score
    |
    v
Store Result
    |
    v
Display Result
```

## Development Methodology

The project follows these development phases:

1.  Requirement Analysis
2.  System and Architecture Design
3.  Database Design
4.  Microservices Development
5.  Frontend Development
6.  API Integration and Testing
7.  System Testing
8.  Deployment and Documentation

## Functional Requirements

-   User registration and login
-   Quiz creation and management
-   Question management
-   Quiz participation
-   Answer submission
-   Automatic evaluation
-   Score calculation
-   Result generation

## Non-Functional Requirements

-   Maintainability
-   Scalability
-   Reliability
-   Security
-   User-friendly interface

## Technical Design

  Layer           Technology / Approach
  --------------- --------------------------
  Frontend        Web-based User Interface
  Backend         Microservices
  Communication   REST APIs
  Database        Centralized Database
  Development     Modern Web Technologies
  Testing         API and System Testing

> The exact programming languages, frameworks, database product, and
> development tools should be updated here once they are finalized in
> the implementation.

## Testing

The project methodology includes:

-   Functional testing
-   API testing
-   Integration testing
-   Database testing
-   System testing

Testing is used to verify individual functionality, service
communication, database operations, and the complete quiz workflow.

## Technical Advantages

-   Modular architecture
-   Separation of major system functionalities
-   Automated quiz evaluation
-   Faster result generation
-   REST API-based communication
-   Easier maintenance
-   Support for future scalability and expansion

## Future Enhancements

Possible future enhancements include:

-   Question randomization
-   Difficulty-based questions
-   Timer-based automatic submission
-   Leaderboard
-   Student performance analytics
-   Admin dashboard
-   Email notification for results
-   Cloud deployment
-   Mobile application

## Project Team

  Name        Student ID
  ----------- ------------
  OM PANDEY   2420030791
  SRUJAN      2420030082
  DHANUSH     2420030788
  MUNUDEEP    2420090018

### Project Guide

**Dr. Navyatha Rani**\
Department of Computer Science and Engineering\
KLH CSE Bowrampet Campus

## Project Status

The project is being developed as part of the **SOA Project Review --
2** for **Batch 5**.

## License

This project is developed for academic purposes.
