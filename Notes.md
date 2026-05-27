### NODE JS

## The “back end”, meanwhile, denotes all that goes on “behind the scenes”
*  If you’re running your own server, you have a ton of flexibility but plenty of headaches. If you’re using the cloud (which we will be doing later), you may be restricted to those languages that your cloud provider has installed on their platform… It doesn’t do you much good if the servers you’re “borrowing” from can’t understand your code!

* most popular server-side languages are PHP, C#, Ruby, Python and Java (not to be confused with JavaScript)

*  back-end can be built in many different programming languages, from compiled languages like Java to interpreted languages like PHP, Python and Ruby.

* Back-end developers also need to interact with database management systems like PostgreSQL, SQL Server, or MySQL. This usually requires knowledge of Structured Query Language (SQL) to read, write, modify, and delete data

* Back-end frameworks like **Flask** or **Django**

* A few popular web technology stacks include:

    * MEAN: MongoDB, Express, Angular, and Node
    * LAMP: Linux, Apache, MySQL, and PHP/Python
    * JAMstack: JavaScript, APIs, and Markup  

***

## What is HTTP?

* HTTP (Hypertext Transfer Protocol) is used to structure requests and responses over the internet. HTTP requires data to be transferred from one point to another over the network. The transfer of resources happens using TCP (Transmission Control Protocol). In viewing this webpage, TCP manages the channels between your browser and the server 

***

## What is an HTTP request?

* HTTP request acts like a conversation starter between a client and server: the client asks for something, and the server replies with either the requested resource or an explanation of why it cannot be provided.

***

### Every HTTP request follows a standard format, which generally includes:

1. Request line: Specifies the HTTP method (e.g., GET, POST), the resource path (e.g., /index.html), and the protocol version (e.g., HTTP/1.1).

* Example: GET /index.html HTTP/1.1

2. Headers: Provide additional context or metadata about the request. Common headers include:

* Host: Indicates the domain name of the server.
* User-Agent: Identifies the client (e.g., Chrome, Firefox).
* Accept: Informs the server what type of content the client can handle (e.g., HTML, JSON).
* Authorization: Sends authentication credentials when accessing protected resources.

3. Body (Optional): Includes data sent to the server, typically in POST, PUT, or PATCH requests. For example, when submitting a login form, the username and password are sent in the body.

* Upon receiving the HTTP request, the server processes it according to the provided instructions. If successful, it responds with an HTTP response that contains:

    * A status code (e.g., 200 OK, 404 Not Found, 500 Internal Server Error)
    * Response headers with metadata
    * An optional response body (such as a webpage, JSON data, or an image)

***

## Types of HTTP requests

* GET: Retrieves data from the server (e.g., loading a webpage).
* POST: Sends data to the server.
* PUT: Updates existing data on the server.
* DELETE: Removes specified data from the server.
* HEAD: Retrieves only headers of a resource, without the actual content.
* PATCH: Applies partial modifications to a resource.
* OPTIONS: Describes communication options available for a resource.

***

## How HTTP requests work

* When you type an address such as www.codecademy.com into your browser, you are commanding it to open a TCP channel to the server that responds to that URL. A URL is like your home address or phone number because it describes how to reach you.

* In this situation, our computer, which is making the request, is called the client. The URL you are requesting is the address which belongs to the server.

* Once the TCP connection gets established, the client sends an HTTP GET request to the server to retrieve the webpage it should display. After the server has sent the response, it closes the TCP connection. If you open the website in your browser again or if your browser automatically requests something from the server, a new connection is opened, which follows the same process described earlier

***

## Note
* DNS (Domain Name Server) 
* IP (Internet Protocol) 

***

* The GET request contains the following text:

    * GET / HTTP/1.1 
    * Host: www.codecademy.com 

***

* If the server is able to locate the path requested, the server might respond with the header:

    * HTTP/1.1 200 OK 
    * Content-Type: text/html 

## HTTP requests vs HTTPS requests

* HTTP requests are suitable only for basic, non-sensitive communication, while HTTPS requests are the secure, trusted standard for modern web interactions.

