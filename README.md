# Serverless_architecture_demo
Serverless architecture is a cloud computing model where you build and run applications without managing servers. The cloud provider handles all infrastructure provisioning, scaling, and maintenance while you focus purely on code.

Function as a Service (FaaS) is the foundation - you write individual functions that execute in response to events. AWS Lambda, Azure Functions, and Google Cloud Functions are the major providers.

Event-driven execution means functions are triggered by events like HTTP requests, database changes, file uploads, message queue events, or scheduled tasks. You only pay for actual execution time.

Stateless functions execute independently without retaining data between invocations. Any state must be stored externally in databases, caches, or object storage.

Architecture Components

Compute layer uses FaaS platforms like AWS Lambda, where functions execute your business logic. API Gateway manages HTTP endpoints and routes requests to appropriate functions. Storage services include object storage (S3), NoSQL databases (DynamoDB), and relational databases (Aurora Serverless). Message queues like SQS, SNS, or EventBridge handle asynchronous communication. Authentication services like Cognito or Auth0 manage user identity.
