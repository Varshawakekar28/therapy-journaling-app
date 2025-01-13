# therapy-journaling-app
# Therapy Journaling App

## Overview
The Therapy Journaling App helps clients maintain emotion journals and allows therapists to manage sessions and interact with journals. The app aims to address the challenges of therapy in remote or isolated conditions, providing tools for clients to express their emotions and for therapists to manage their growing clientele efficiently.

## Features
- **Clients:**
  - Create and manage their accounts.
  - Maintain an emotions journal, adding records of feelings and their intensities.
  - Search for and connect with therapists.
  - Manage therapist access to their journals.
  - Schedule and manage therapy appointments.
- **Therapists:**
  - View client journals (with authorization).
  - Create therapy sessions with private and shared notes.
  - Send and receive messages with clients.
  - Manage a list of mapped clients.

## Setup Instructions

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/therapy-journaling-app.git
    ```
2. Navigate to the project directory:
    ```bash
    cd therapy-journaling-app
    ```
3. Set up the environment and dependencies:
    - Ensure you have the AWS CLI installed and configured.
    - Install Java 11 and Maven.
4. Deploy the application:
    - Use AWS CDK to deploy the backend services.
5. Test the APIs:
    - Import the Postman collection located in `WebDev/backend/` and run tests.

## How to Run

1. Ensure AWS CLI is installed and configured:
    ```bash
    aws configure
    ```
2. Deploy the application using AWS CDK:
    ```bash
    cdk deploy
    ```
3. Use Postman to test the APIs:
    - Open Postman.
    - Import the collection from `WebDev/backend/postman_collection.json`.
    - Use the sample requests to test each endpoint.

## API Documentation

The API is designed using Swagger and adheres to the OpenAPI 3.0 specification. Key resources include:
- **Clients**:
  - `POST /clients`: Create a new client account.
  - `GET /clients/{clientId}`: Fetch details for a specific client.
  - `PUT /clients/{clientId}`: Update client details.
  - `DELETE /clients/{clientId}`: Delete a client account.

- **Therapists**:
  - `POST /therapists`: Create a new therapist account.
  - `GET /therapists/{therapistId}`: Fetch details for a specific therapist.
  - `PUT /therapists/{therapistId}`: Update therapist details.
  - `DELETE /therapists/{therapistId}`: Delete a therapist account.

For the full Swagger definition, refer to `WebDev/backend/swagger.yaml`.

## Technology Stack

- **Programming Language**: Java
- **Cloud Platform**: AWS Lambda, DynamoDB, API Gateway
- **API Design**: Swagger/OpenAPI
- **Testing**: Postman

## Contributing

We welcome contributions to improve this project. Please follow these steps:
1. Fork this repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-name
    ```
3. Commit your changes:
    ```bash
    git commit -m "Add feature-name"
    ```
4. Push to your forked repository:
    ```bash
    git push origin feature-name
    ```
5. Create a pull request and describe your changes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.


