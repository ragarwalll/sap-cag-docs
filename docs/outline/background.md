### Requirements

Launching a new project or proof of concept (POC) can be a time-consuming and challenging task, especially when it comes to setting up the full stack, including the frontend, backend, and local setup and deployment descriptors. The process often involves extensive research and effort to produce a deployment-ready codebase. While various tools address different aspects of the setup process, there isn't a single solution that provides a comprehensive, end-to-end deployment-development ready codebase.

Developing a full-stack codebase that utilizes `UI5/React` for the frontend and `NodeJS/Spring Boot` for the backend, with the capability to deploy in `SAP BTP`, can be a complex and demanding task. Integrating multiple technologies in a single codebase, while ensuring proper compatibility and deployment in `SAP BTP`, can present significant challenges

`SAP BTP` offers services for authentication and authorization to applications, which can be consumed to enable these features. However, even after setting up the codebase, manual consumption of these services may be required within the application to fully enable authentication and authorization.

In the same vein, there are some common services that are utilized across SAP products, and their setup is generally similar.

### Solutions Proposal

To address this challenge, we proposed creating a `boilerplate generator`. This generator would provide a guided flow for the user, allowing them to choose their preferred frontend and backend framework, as well as opting in to use `SAP BTP services` for authentication and authorization. This way, the generator would offer a streamlined process for setting up a full-stack codebase and integrating necessary services.

To ensure accessibility for users, the application can be presented as either a `Command Line Interface (CLI)` extension or a `Graphical User Interface (UI)` application. Currently, with most users utilizing `Visual Studio Code (VSCode)` as their primary `Integrated Development Environment (IDE)`, the application can be made available as a `VSCode plugin extension`.

The concept is to have a centralized codebase by abstracting the underlying logic. This will allow us to have an API or extension that targets the generator as either a `VSCode extension`, a `Graphical User Interface (UI)` application, or a `Command Line Interface (CLI)` plugin, resulting in a unified solution.

### Relevance of the project in SAP

At `SAP`, we initiate multiple projects and `Proof-of-Concepts (PoCs)` daily. Regardless of whether the employee is at an entry-level or an experienced level, the setup for these projects is typically standardized and time-consuming. Our focus is primarily on deploying our applications to the `SAP Business Technology Platform (BTP)` and utilizing its extensive array of services. To accomplish this, we primarily use the `SAP Cloud MTA tool`, which enables us to deploy a fully stacked application in one go. In conclusion, the process involved, starting from modifying code to be compatible with `BTP`, to creating deployments for various environments, is repetitive and labor-intensive.

By utilizing this tool, we anticipate significant time savings in the setup of projects, which typically requires several days or even weeks to complete.