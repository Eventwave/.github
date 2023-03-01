# TicketFlow

TicketFlow is an event and ticket management application that uses microservices technology to provide a scalable and secure event management environment.

The application is built using different technologies, including Flyway, MongoDB and Postgres for data management, Kafka for communication between microservices, Border Gateway to ensure secure access to services and Discovery to ensure that each service can be discovered and accessed by other services in a secure and scalable way.

## Microservices

The TicketFlow application is made up of different microservices, each with its own responsibility and functionality:

* Authentication service
* Event management service
* Ticket management service
* Booking management service
* Payment processing service
* Notification service
* Sales analysis service

Each microservice is deployed in a Docker container, which makes it easy to manage and deploy across different environments. Containers can be easily scaled horizontally according to demand.
## Tables and collections
Below are some of the tables and collections used by the TicketFlow application, along with their relationships:

**Users:** table to store information about users accessing the application, including name, email address, encrypted password, creation and update date.

**Events:** collection to store information about events registered on the platform, including name, description, location, date, time, capacity, image, category and additional details of the event.

**Tickets:** table to store information on tickets available for sale in each event, including the event to which it belongs, the name, price, available quantity and creation and update dates.

**Reservations:** table to store information on ticket reservations made by users, including the user who made the reservation, reserved ticket, quantity, status (pending, confirmed or cancelled) and creation and update dates.

In addition to these tables and collections, the TicketFlow application also uses other tables and collections to store additional information about users, events and reservations.
## Using Docker
To deploy and run the TicketFlow application, you need to configure and start each microservice individually, ensuring that they are all communicating correctly. Each microservice has its own configuration and set of dependencies, which must be managed separately.

For easy management and deployment in different environments, each microservice is deployed in a Docker container. Docker allows each service to run in an isolated and independent environment, making it easy to deploy and scale.

## Installation
To install and run the TicketFlow application, follow these steps:

1.  Clone the Github repository for your development environment.
2. Make sure you have Docker installed on your machine.
3. Start each microservice with the docker-compose up command.
4. Access the application in your browser at http://localhost:8080.

## Contribution
If you would like to contribute to the TicketFlow application, please follow these steps:

1. Fork the Github repository.
2. Clone the repository to your development environment.
3. Make the desired changes on a new branch.
4. Open a pull request for review.

## Contact
For any questions or suggestions, please contact us at daniellygj@gmail.com.
