## Getting Started

Welcome to the documentation for the `SAP Cloud Application Generator`.

This powerful tool enables you to quickly `scaffold` applications, allowing you to build functional apps in a matter of minutes. With our `intuitive interface`, you have convenient access to a range of `frontend` and `backend` packages, making the app scaffolding process effortless and efficient.

### Why this?

When it comes to developing and deploying apps in [SAP Business Technology Platform (BTP)](https://www.sap.com/india/products/technology-platform.html), the process of building a ready-made app can be quite tedious.

#### Frontend

Currently, there are a few options available for building UI apps:

1. `Deploying Static Files`: One approach is to deploy the static files directly within the app. This means including the necessary HTML, CSS, and JavaScript files in the app itself. Alternatively, you can deploy these files to the [HTML5 repository](https://help.sap.com/docs/btp/sap-business-technology-platform/html5-application-repository) and utilize the [Approuter](https://help.sap.com/docs/btp/sap-business-technology-platform/application-router), which serves as a proxy to route requests to the correct destination.

1. `Utilizing Existing Generators`: Another option is to leverage the existing generator tools that are available. These generators provide a streamlined way to quickly scaffold UI apps by generating the necessary code and project structure based on predefined templates. This can significantly reduce manual effort and speed up the development process.

Both approaches have their advantages and can be chosen based on the specific requirements and preferences of the `development team`.

When it comes to developing `backend` apps, the `XSUAA` service in `SAP BTP` is commonly used for `authorization` and `authentication`. However, depending on the programming language you choose, the setup process may vary in length and complexity.

#### Backend

Setting up XSUAA service for authorization and authentication typically involves the following steps:

1. `Configuring Security`: You need to define security configurations in the [XSUAA](https://sap.github.io/cloud-sdk/docs/java/guides/cloud-foundry-xsuaa-service) service instance with the available libraries out there.

2. `Implementing Authorization and Authentication Logic`: Once the integration is in place, you will need to implement the authorization and authentication logic within your backend application. This includes validating tokens, checking scopes and permissions, and enforcing security rules to protect sensitive data and endpoints.

The complexity and duration of these steps may vary depending on the specific backend language and frameworks you are working with. It is recommended to consult the documentation and resources specific to your chosen language to ensure a smooth setup process for `XSUAA` service integration.

#### Intergration

Indeed, after setting up both the `frontend` and `backend` components, it is essential to properly configure the `destinations` for seamless interaction between them. This applies to both local development and deployment scenarios.

Destinations serve as connection points that define the endpoints and connectivity details of the backend services. They allow the frontend application to communicate with the backend, enabling data retrieval, manipulation, and other interactions.

For local development, you typically configure destinations to connect the frontend application running on your local machine with the backend services deployed either locally or remotely. This involves specifying the `destination URL`,` authentication details`, and other necessary parameters. The exact process may vary depending on the development environment and tools you are using.

During deployment, the destination configurations need to be adjusted to match the deployment environment. This includes updating the destination URLs, authentication credentials, and other relevant settings to ensure proper communication between the frontend and backend services.

It's important to ensure that the destination configurations are accurate and up to date, as any misconfiguration can result in communication errors or failed interactions between the frontend and backend components.

Consulting the documentation specific to your development environment, such as `SAP BTP`, can provide detailed guidance on configuring destinations for both local development and deployment scenarios.

!!! example "TL;DR"

    Setting up the full stack for `development` and `deployment` can indeed be a challenging task. However, with our tool, this process becomes incredibly simplified, requiring just `one click`.