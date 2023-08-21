# API Introduction

<sub>_This section is a very basic overview of what an API is. If you're familiar with APIs, you can skip to the next guide._</sub>

An API (Application Programming Interface) is a collection of protocols, tools, and definitions used for building software and applications. It enables different software systems or components within a system to communicate and interact with each other.

The most common type of API is a web API, which is accessed through HTTP requests and responses, utilizing various programming languages.

## Anatomy of an API Request

An API request consists of the following components:

-   **Endpoint**: The URL that specifies the target location for the request.
-   **Request Body**: Contains the data being sent, usually formatted in JSON.
-   **Method**: The HTTP method or "verb" used to interact with the API. The most common methods are:
    -   **GET**: Retrieves data from the API.
    -   **POST**: Submits data to the API for processing.
    -   **PUT**: Updates existing data on the API.
    -   **DELETE**: Removes data from the API.

Additionally, API requests often include an authentication header to verify the client's authorization and protect sensitive information.

## Anatomy of an API Response

An API response consists of the following elements:

-   **Response Code**: A numerical code indicating the status of the API request.
-   **Response Body**: Contains the data returned by the API, usually formatted in JSON.

Common response codes include:

-   **200 OK**: The request was successful, and the requested data is included in the response.
-   **400 Bad Request**: The request was malformed or invalid.
-   **401 Unauthorized**: Authentication is required, but the provided credentials were invalid or missing.
-   **403 Forbidden**: The request is not allowed, even with valid credentials, due to insufficient permissions or access restrictions.
-   **404 Not Found**: The requested resource could not be found on the server.
-   **500 Internal Server Error**: The server encountered an error while processing the request.

## Analogy: The Restaurant Example

Imagine being in a restaurant, examining the menu and deciding what to order. The menu represents the API documentation, providing a list of available options.

You communicate your order to the waiter, who relays it to the kitchen. This corresponds to making an API request.

The kitchen prepares the food and returns it to the waiter, who then serves it to you. Similarly, the API processes your request and delivers the desired data back to your application.

In this analogy, the restaurant represents the API provider, the kitchen represents the backend systems handling the request, the waiter represents the API itself, and you represent the application making the request.

Just as a waiter's actions depend on the restaurant's offerings, an API can only provide access to the functionality and data permitted by the underlying system. You can use different APIs, just as you can visit various restaurants with different menus.

Let's extend this analgy to the request methods:

-   **GET**: Asking the waiter for a menu, similar to making a `GET` request to retrieve data.
-   **POST**: Ordering a pizza by informing the waiter, like making a `POST` request to submit data.
-   **PUT**: Requesting the kitchen to cook your pizza longer, similar to making a `PUT` request to update existing data.
-   **DELETE**: Canceling your pizza order through the waiter, akin to making a `DELETE` request to remove data.

The response codes can also fit into the restaurant analogy:

-   **200 OK**: Requesting water and receiving it without issues, like receiving a `200 OK` response.
-   **400 Bad Request**: Requesting raw meat, which is not allowed, similar to receiving a `400 Bad Request` response for an invalid or malformed request.
-   **401 Unauthorized**: Trying to order a VIP-only dish without the necessary credentials, leading to a `401 Unauthorized` response.
-   **403 Forbidden**: Attempting to enter the kitchen as a customer, resulting in a `403 Forbidden` response due to access