# Hotel Ratings Platform
## Microservices:
Microservices architecture is a style of building software systems that are composed of small, independent services that communicate over well-defined APIs. These services are independently deployable and scalable, making it easier to develop, test, deploy, and scale complex applications.
Java is a popular language for building microservices due to its robustness, extensive ecosystem, and strong community support.
### User Service
Created User Microservice using MYSQL Database and tested API using POSTMAN.
### Hotel Service
Created Hotel Microservice using PostgreSQL Database and tested API using POSTMAN.
### Rating Service
Created Rating Microservice using MongoDB Database and tested API using POSTMAN.

# Demonstration Of the Project:
 
<img width="678" alt="Capture" src="https://github.com/anjalikhushi/Hotel-Microservice-App/assets/82653640/0044dbaa-7ebe-42de-bba3-f7d771275f88">

# Explanation 
#### Service Registry
It is a database or a service that maintains the information about the available services, their instances, and their locations. This allows microservices to discover and communicate with each other dynamically, enhancing scalability and flexibility.
##### Eureka Server
Eureka is a service registry developed by Netflix as part of its Netflix OSS stack. It is used to register services and allow other services to discover them. 
## Open Feign Client
Feign is a declarative web service client that makes writing web service clients easier. It integrates seamlessly with Spring Cloud and Eureka, allowing you to write web service clients with just a few lines of code. Here's how you can set up and use a Feign client in a Spring Boot application.
## API Gateway
An API Gateway is an essential component in a microservices architecture. It acts as a reverse proxy to accept all application programming interface (API) calls, aggregate the various services required to fulfill them, and return the appropriate result. It can handle requests by routing them to the appropriate microservices, applying security, throttling, load balancing, and caching.
## Handling Fault Tolerance Using Resilience4j:
### Resilience4j
Resilience4j is a lightweight fault tolerance library inspired by Netflix Hystrix but designed for Java 8 and functional programming. It provides various fault tolerance mechanisms such as Circuit Breaker, Rate Limiter, Retry, Bulkhead, and TimeLimiter.
# Securing Microservices
### OktaAuth:
Integrating Okta for authentication in a Spring Boot application enhances security by providing secure access to your application with minimal configuration. Okta handles user authentication, authorization, and user management, which makes it easier to implement secure login functionality in your application. Here's a step-by-step guide to integrating Okta authentication in a Spring Boot application.

## Prerequisites
1.Okta Developer Account: Sign up for a free Okta developer account at developer.okta.com.

2.Spring Boot Application: Have a Spring Boot application ready.

3.Create an Okta Application.

4.Log in to Okta: Log in to your Okta account.

## Create a new Application:

1.Go to Applications > Add Application.

2.Select Web as the platform.

3.Click Next.

## Configure your Application:

1.Enter a name for your application.

2.Set Login redirect URIs to http://localhost:8080/login/oauth2/code/okta.

3.Click Done to create the application.

4.Get Client ID and Secret:

Once the application is created, you will see the Client ID and Client Secret on the application's page. Keep these values handy as they will be used in your Spring Boot application.

## Creating and Configuring a RestTemplate Interceptor:
Using a RestTemplate interceptor allows you to add pre-processing and post-processing logic for your HTTP requests and responses. This can be very useful for cross-cutting concerns such as logging, authentication, or modifying requests and responses.
## Steps:
1.Add Dependencies.

2.Create an Interceptor.

3.Configure the RestTemplate to Use the Interceptor.

4.Use the Configured RestTemplate

