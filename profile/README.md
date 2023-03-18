# TicketFlow

TicketFlow is a comprehensive ticketing system designed to manage event ticket sales. The project is built using microservices architecture, utilizing services such as Border Gateway, Eureka, Config Server, and RabbitMQ for effective communication and data flow between the services.

![diagrama](https://github.com/TicketFlow/.github/blob/main/utils/diagrama.png)


Services Overview
The system is comprised of several services, each responsible for handling specific aspects of the ticketing process.

* **CouponManager**: Manages discount coupons that can be applied during the checkout process.
* **Authentication**: Handles user authentication and authorization for accessing the platform.
* **TicketManager**: Manages the tickets available for sale for each event, including adding, removing, and updating tickets.
* **PaymentProcessing**: Processes payments for ticket reservations.
* **EventManager**: Manages events, including adding, removing, and updating events.
* **SalesManager**: Manages the shopping cart and sales transactions.
* **SalesAnalytics**: Analyzes sales data and provides useful insights for business decision-making. Generates reports on popular events, top-selling tickets, and overall revenue.
* **Notification**: Sends event notifications to users.

### Border Gateway
The Border Gateway is the entry point for all client requests. It is responsible for routing requests to the appropriate microservices and handling any errors or exceptions that may occur. This layer provides an additional level of security by filtering out malicious requests and enabling the implementation of authentication and rate-limiting policies.

### Eureka
Eureka is a service registry and discovery tool used in this project to manage the microservices. It enables each microservice to discover and communicate with other microservices, providing load balancing and fault tolerance.

### Config Server
The Config Server centralizes configuration data across all microservices, ensuring consistent configuration settings for each service. This enables easy management and updating of configurations without the need to restart services or redeploy the system.

### RabbitMQ
RabbitMQ is a message broker used for communication between microservices. It ensures reliable and efficient data transfer, allowing for asynchronous communication and decoupling of services.

### Docker and Docker Compose
Docker is used to package each microservice into a container, providing an isolated environment that includes all dependencies required for the service to run. This ensures consistency across development, testing, and production environments, and simplifies the deployment process.
It is used to define and manage the entire system, including all microservices and their dependencies. It allows for easy deployment, scaling, and management of the services using a single configuration file.

## Contribution
If you would like to contribute to the TicketFlow application, please follow these steps:

1. Fork the Github repository.
2. Clone the repository to your development environment.
3. Make the desired changes on a new branch.
4. Open a pull request for review.

## Contact
For any questions or suggestions, please contact us at daniellygj@gmail.com.
