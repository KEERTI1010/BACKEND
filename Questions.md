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

***