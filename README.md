# Best Buy Cloud Native Application
Welcome to the Best Buy Cloud-Native Demo Application, a microservices-based reference system built using the Algonquin Pet Store (On Steroids) architecture. This project represents a realistic, production-style cloud-native application designed to demonstrate modern full-stack development, containerization, and Kubernetes orchestration patterns.


## Architecture

The application has the following services: 

| Service | Description | Github Repo |
| --- | --- | --- |
| `store-front` | Web app for customers to place orders (Vue.js) | [store-front-L8](https://github.com/ramymohamed10/store-front-L8) |
| `store-admin` | Web app used by store employees to view orders in queue and manage products (Vue.js) | [store-admin-L8](https://github.com/ramymohamed10/store-admin-L8) |
| `order-service` | This service is used for placing orders (Javascript) | [order-service-L8](https://github.com/ramymohamed10/order-service-L8) |
| `product-service` | This service is used to perform CRUD operations on products (Rust) | [product-service-L8](https://github.com/ramymohamed10/product-service-L8) |
| `makeline-service` | This service handles processing orders from the queue and completing them (Golang) | [makeline-service-L8](https://github.com/ramymohamed10/makeline-service-L8) |

The application uses MongoDB as a stateful data store, deployed alongside stateless services, to demonstrate real-world data persistence considerations in Kubernetes environments.

This demo emphasizes:
- Microservices and API-first design
- Event-driven communication patterns
- Containerization and Kubernetes deployment
- Separation of concerns between frontend, backend, and worker services
- Realistic cloud-native operational architecture suitable for enterprise environments like Best Buy

![Logical Application Architecture Diagram](assets/Algonquin%20Pet%20Store%20On%20Steroids.png)

## Run the app on Azure Kubernetes Service (AKS)

You can use the kubernetes YAML files provided in the [Deployment Files](./Deployment%20Files/) folder to deploy the app to an AKS cluster.



