## Introduction
This project is a demonstration of a GraphQL API gateway integrating with REST APIs and gRPC microservices. It includes functionality for managing suppliers and products.

## Getting Started

### Prerequisites
- Node.js installed on your machine
- npm package manager

### Installation
1. Download the project repository to your local machine.
2. Open the project directory in Visual Studio Code.

### Running the Project
1. Open three terminals in Visual Studio Code.
2. In the first terminal, navigate to the project root directory and run the following command to start the REST API:
npm start


3. In the second terminal, navigate to the "microservices" folder "cd microservices" and run the following command to start the supplier microservice:

node supplierMicroservice.js


4. In the third terminal, repeat step 3 but for the product microservice:
node productMicroservice.js


### Testing
1. Open Postman and create a new HTTP request to interact with the REST API. You can find the available routes in the "test.js" file.(localhos:3000)
2. Open a GraphQL client window on port 4000 to test the GraphQL API.
3. Open another window in your gRPC client and import the "product.proto" file from the project. Specify the port as 50054.
4. Import the "supplier.proto" file in the gRPC client window and specify the port as 50053.
5. Enjoy testing the functionality of the project!

## Dependencies
- apollo-server: for implementing the GraphQL server.
- express: for building the REST API.
- @grpc/grpc-js: for creating gRPC clients.
- @grpc/proto-loader: for loading Protobuf definitions.
- mongoose: for interacting with MongoDB.
- cors: for enabling CORS in the REST API.
- nodemon: for automatically restarting the server during development.

## Additional Notes
Make sure to install all dependencies using npm before running the project.