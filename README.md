# REST API Simple Example

This is a RESTful API example based on Node.js and MongoDB, following the **MVC pattern** i.e. Model ~~View~~ Controller.

**Mongoose** is used for Database transactions which is an elegant solution to mongodb object modeling for node.js.

The application is **production ready**, and can be used behind a Nginx reverse proxy securely.

## Prerequisites

Make sure you have the following prerequisites installed on your machine:

- Docker: [https://www.docker.com/](https://www.docker.com/)

## Configuration

Before running the application, make sure to configure the following files and environment variables:

- `.env`: Environment variable file for application configuration. Refer to `.env.example` file for an example and make sure to provide the appropriate values for your environment.

## Installation

Follow these steps to install and run the application:

1. Clone the application repository from GitHub:

```bash
git clone https://github.com/manupaiva/node-rest-api-nvc-docker.git
```

2. Navigate to the application directory:

```bash
cd NODEJS-REST-API
```

## Execution

Follow these steps to run the application:

1. Build the application using Docker build:

```bash
docker build .
```

2. Start the Docker containers using Docker Compose:

```bash
docker compose up -d
```

This will start the containers for your API and MongoDB, ensuring their connection.

3. Access the API in your browser or using tools like Postman:

```bash
http://localhost:CONTAINER_PORT/
```

Make sure to replace CONTAINER_PORT with the port configured in your .env file.

## Usage

To use this API you have an example queries in rest.http file.

## Author

- [**Manuel Paiva**](https://github.com/manupaiva)

## License

This project is licensed under the MIT License.
