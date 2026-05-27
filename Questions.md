# HTTP

```jsx
1. What are the 7 HTTP methods?
The 7 HTTP request methods include:

GET: Retrieves data from the server (e.g., loading a webpage).
POST: Sends data to the server.
PUT: Updates existing data on the server.
DELETE: Removes specified data from the server.
HEAD: Retrieves only headers of a resource, without the actual content.
PATCH: Applies partial modifications to a resource.
OPTIONS: Describes communication options available for a resource.
```

```jsx
2. What is in an HTTP request?
An HTTP request typically contains:

1. Request line: Specifies the HTTP method (e.g., GET, POST), the resource path (e.g., /index.html), and the protocol version (e.g., HTTP/1.1).

Example: GET /index.html HTTP/1.1
2. Headers: Provide additional context or metadata about the request. Common headers include:

Host: Indicates the domain name of the server.
User-Agent: Identifies the client (e.g., Chrome, Firefox).
Accept: Informs the server what type of content the client can handle (e.g., HTML, JSON).
Authorization: Sends authentication credentials when accessing protected resources.
3. Body (Optional): Includes data sent to the server, typically in POST, PUT, or PATCH requests. For example, when submitting a login form, the username and password are sent in the body.
```

```jsx
3. What is HTTP used for?
HTTP is used for:

Transferring web content (HTML, CSS, JavaScript, images, videos, etc.) between clients (like browsers) and servers
Enabling communication for REST APIs and many web services
Building the foundation of the World Wide Web
```

```jsx
4. What is the difference between HTTP and TCP?
HTTP is an application-layer protocol that defines how messages are formatted and transferred over the web.
TCP is a transport-layer protocol that ensures reliable data delivery between devices
```

```jsx
5. What is the difference between HTTP request and API request?
An HTTP request is a general request for web resources like pages, images, or scripts, usually made by browsers and returning content for users.
An API request is a specific type of HTTP request that targets an API endpoint, typically returning structured data like JSON or XML for use by applications or services.
```

```jsx
https://www.codecademy.com/article/what-is-http
```

***

# REST

```jsx
1. What do you mean by REST API?
A REST API is a special kind of interface that enables clients and servers to communicate using a set of REST principles based on HTTP methods, statelessness, and resource representation. It exposes resources through endpoints, usually returning data in formats like JSON or XML.
```

```jsx
2. What’s the difference between API and REST API?
An API is a general term that refers to any interface that allows software applications to communicate with each other. A REST API is a particular type of API that follows REST principles—using HTTP methods, stateless communication, and resource-based endpoints. In short, all REST APIs are APIs, but not all APIs are REST APIs.
```

```jsx
3. Is REST API just HTTP?
No. REST is an architectural style, not a protocol. While most REST APIs use HTTP as the transport protocol, REST principles can be applied over other protocols too. However, HTTP has become the most common choice due to its simplicity and wide adoption.
```

```jsx
4. Do all REST APIs use JSON?
No. JSON is the most popular format because it is lightweight, easy to read, and well-supported by modern programming languages. However, REST APIs can return other formats such as XML, YAML, or even plain text, depending on the client’s Accept header and the server’s implementation
```

```jsx
5. Do REST APIs use XML?
Yes, REST APIs can use XML. In fact, before JSON became dominant, XML was widely used as the standard data format for REST APIs. While JSON is now more common, some APIs still support XML, particularly in enterprise or legacy systems
```

```jsx
https://www.codecademy.com/article/what-is-rest-api
```

# Backend_ Architecture

```jsx
1. What are the main components of back-end architecture?
The three main components are the server (computer that receives requests), the application (software that processes requests and contains business logic), and the database (system that stores and organizes data persistently).
```

```jsx
2. How does back-end architecture differ from front-end?
Front-end architecture focuses on what users see and interact with in their browsers, while back-end architecture handles data processing, storage, and server-side logic that happens behind the scenes to support the user interface.
```

```jsx
3. What programming languages are used in back-end development?
Popular back-end programming languages include JavaScript (Node.js), Python, Java, PHP, Ruby, C#, and Go. The choice depends on project requirements, team expertise, and performance needs.
```

```jsx
4. Why is database integration important in back-end architecture?
Databases provide persistent storage for application data, reduce server memory load, and ensure data survives server crashes. They enable applications to store user information, content, and business data reliably over time
```

```jsx
5. What is the role of APIs in back-end architecture?
APIs (Application Programming Interfaces) define how different software components communicate. In back-end architecture, APIs expose endpoints that allow front-end applications and external services to request and send data to the server
```

```jsx
https://www.codecademy.com/article/what-is-back-end-architecture
```
