# DIGI-EDGE

Welcome to the DIGI-EDGE organization! This organization houses multiple repositories that contain various services designed to interact with each other in order to collect data from multiple devices using serial port or MQTT protocol and forward the decoded data to external MQTT brokers. Our projects include DPE-FRONT, DPE-BACK, DPE-RULE-ENGINE, DPE-REAL-TIME, services that forward data from a serial port or via MQTT to a RabbitMQ queue and forward data to an external MQTT broker, and rule engine sevice. Below you'll find an overview of the organization and a brief description of each repository.

## Overview

Our organization aims to provide a comprehensive suite of services that enable seamless communication and data processing. The repositories are structured as follows:

1. **Frontend**
   - Repository: `DPE-FRONT`
   - Description: This repository contains the front-end codebase that interacts with the back-end and displays data to end-users. It provides a user-friendly interface for data visualization and interaction.

2. **Backend**
   - Repository: `DPE-BACK`
   - Description: The `digi-backend` repository holds the code for the back-end service. It manages data processing, manages devices and other options, communicates with the front-end and other services.

3. **Serial to queue forwarding**
   - Repository: `DPE-SERIAL-QUEUE`
   - Description: This repository hosts the service responsible for forwarding data from the serial port to a RabbitMQ queue. It ensures reliable and asynchronous data transfer for downstream processing.

4. **MQTT to queue forwarding**
   - Repository: `DPE-MQTT-QUEUE`
   - Description: This repository hosts the service responsible for forwarding data arrived via MQTT protocol to a RabbitMQ queue.

5. **Rule Engine**
   - Repository: `DPE-RULE-ENGINE`
   - Description: The `DPE-RULE-ENGINE` repository hosts the service responsible for managing and executing business rules and logic within our system. This service plays a crucial role in automating decisions, actions, and data processing based on predefined rules and conditions.

6. **Real time forwarding**
   - Repository: `DPE-REAL-TIME`
   - Description: The `DPE-REAL-TIME` repository contains the codebase for our Real-Time Data Dashboard Service. It acts as a bridge between the backend processing services and the frontend application, ensuring that real-time data updates are efficiently delivered to the user's dashboard.

7. **External brokers forwarding**
   - Repository: `DPE-MQTT-FWD`
   - Description: The `DPE-MQTT-FWD` repository holds the code for the service responsible for forwarding processed data to an external MQTT broker. This allows integration with external systems and dashboards.

## Getting Started

To get started with any of our services, follow the steps below:

1. Clone the repository of the service you wish to work with to your local development environment.

2. Review the documentation available in each repository for detailed information on how the services operate and interact with each other.

3. Ensure you have the necessary dependencies and requirements installed as specified in each repository's documentation.

4. Run the services in the recommended order to establish communication and interaction between them. Typically, the flow would be from the `DPE-SERIAL-QUEUE` or `DPE-MQTT-QUEUE` through `DPE-BACK` to either the `DPE-RULE-ENGINE` service and then finally to the `DPE-MQTT-FWD` and `DPE-REAL-TIME`.

![DIGI-EDGE Schema Flow](https://github.com/DIGI-EDGE/.github/blob/main/profile/DIGIEDGE.png)

5. Contribute to the repositories by creating pull requests for new features, bug fixes, or improvements. Please adhere to our code style guidelines and submit well-documented code.

6. Join our community discussions to get help, share ideas, and collaborate with other contributors.

## Community and Support

We believe in an open and inclusive community where everyone is welcome to participate. If you have questions, encounter issues, or want to engage with other developers, you can:

- Join our community Slack/Discord channel (link available in each repository's documentation).
- Raise issues or bug reports in the respective repository.
- Contribute to ongoing discussions and propose new ideas on our community forums.

## License

All repositories under the DIGI-EDGE organization are released under the [MIT License](https://opensource.org/licenses/MIT). Please review the specific license files in each repository for more details.

Thank you for choosing DIGI-EDGE! We hope our services help you build amazing projects and applications. Happy coding! 🚀
