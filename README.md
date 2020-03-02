AWS Serverless Ecommerce Platform
=================================

The __Serverless Ecommerce Platform__ is a sample implementation of a serverless backend for an e-commerce website. Functionalities are split across multiple micro-services that communicate either through asynchronous messages over [Amazon EventBridge](https://aws.amazon.com/eventbridge/) or over synchronous APIs.

<p align="center">
  <img src="docs/images/flow.png" alt="High-level flow across microservices"/>
</p>

## Getting started

To install the necessary tools and deploy this in your own AWS account, see the [getting started](docs/getting_started.md) guide in the documentation section.

## Backend services

|  Services  | Description                               |
|------------|-------------------------------------------|
| [Users](users/) | Provides user management, authentication and authorization. |
| [Products](products/) | Source of truth for products information. |
| [Orders](orders/) | Manages order creation and status. |
| [Warehouse](warehouse/) | Manages inventory and packaging orders. |
| [Delivery](delivery/) | Manages shipping and tracking packages. |
| Payment | Manages payment collection and refunds. |

## Frontend service

|  Services  | Description                               |
|------------|-------------------------------------------|
| Frontend | Web interface for interacting with the services. |

## Infrastructure services

|  Services  | Description                               |
|------------|-------------------------------------------|
| [Pipeline](pipeline/) | CI/CD pipeline for deploying the resources in production. |
| [Platform](platform/) | Core platform resources for deploying backend services. |

## Shared resources

| Name       | Description                               |
|------------|-------------------------------------------|
| [Docs](docs/) | Documentation application for all services. |
| [Shared](shared/) | Shared resources accessible for all services, such as common CloudFormation templates and OpenAPI schemas. |
| [Tools](tools/) | Tools used to build services.             |


## Documentation

See the [docs](docs/) folder for the documentation.

## Contributing

See the [contributing](CONTRIBUTING.md) and [getting started](docs/getting_started.md) documents to learn how to contribute to this project.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
