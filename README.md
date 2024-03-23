# Task Tracker Info

## Overview

General information for the Task - Tracker Micro Service Application

The project's technical specifications are
taken [here](https://zhukovsd.github.io/java-backend-learning-course/Projects/TaskTracker/).

### Microservices:

- Service Discovery [here](https://github.com/Bityta/task-tracker-service-discovery).
- Email Sender [here](https://github.com/Bityta/task-tracker-email-sender)
- Backend [here](https://github.com/Bityta/task-tracker-backend).
- Scheduler [here](https://github.com/Bityta/task-tracker-scheduler).

## Microservices Startup Sequence:

### Service Discovery:

Begin by launching the Service Discovery microservice. This component acts as a registry for all available services
within the system. Ensure that the Service Discovery microservice is up and running before proceeding to the next step.

### Email Sender:

Next, start the Email Sender microservice. This service is responsible for sending out welcome emails to users upon
successful registration. It integrates with external email services to deliver emails reliably. Wait for the Email
Sender microservice to initialize and establish connections.

### Backend:

Once the Service Discovery and Email Sender microservices are operational, initiate the Backend microservice. This is
the core of the application, providing REST API endpoints for user management and task tracking functionalities. Ensure
that the Backend microservice successfully registers itself with the Service Discovery component for seamless service
discovery.

### Scheduler:

Finally, launch the Scheduler microservice. This component is responsible for scheduling tasks and managing their
execution. It integrates with the Backend microservice to retrieve task data and execute scheduled actions as per user
requirements. Wait for the Scheduler microservice to establish connections with the Backend microservice and synchronize
task data.
Ensure that all microservices are started in the specified sequence to maintain proper functionality and inter-service
communication within the application ecosystem. Monitor the startup logs of each microservice for any errors or issues
that may arise during initialization. Once all microservices are up and running, the application should be ready to
handle user registrations, task management, and scheduled actions effectively.
