# NODE

* an asynchronous event-driven JavaScript runtime, Node.js is designed to build scalable network applications

* Node allows you to run JavaScript code on a machine such as your local computer or a server without having to go through a web browser

* **Undici** is an HTTP client library that powers the **fetch API** in Node.js. It was written from scratch and does not rely on the built-in HTTP client in Node.js. It includes a number of features that make it a good choice for high-performance applications

* Node.js is called asynchronous and event-driven because it does not wait for one task to finish before starting another task


## What is a web server?
* The term web server can refer to hardware or software, or both of them working together
    * On the hardware side, a web server is a computer that stores web server software and a website's component files (for example, HTML documents, images, CSS stylesheets, and JavaScript files). A web server connects to the Internet and supports physical data interchange with other devices connected to the web.
    * On the software side, a web server includes several parts that control how web users access hosted files. At a minimum, this is an HTTP server. An HTTP server is software that understands URLs (web addresses) and HTTP (the protocol your browser uses to view webpages). An HTTP server can be accessed through the domain names of the websites it stores, and it delivers the content of these hosted websites to the end user's device

* At the most basic level, whenever a browser needs a file that is hosted on a web server, the browser requests the file via HTTP. When the request reaches the correct (hardware) web server, the (software) HTTP server accepts the request, finds the requested document, and sends it back to the browser, also through HTTP. (If the server doesn't find the requested document, it returns a 404 response instead.)

## Dedicated web server
* A dedicated web server can have the same IP address all the time. This is known as a dedicated IP address. (Not all ISPs provide a fixed IP address for home lines.)
* A dedicated web server is typically maintained by a third party

## how to make our website live
### File Upload Software

* Used to upload website files to a web server.

    * Examples:
        1.FileZilla
        2.WinSCP

* Main Process
    * Write website code in text editor.
    * Test website in browser.
    * Upload files to web server using FTP/SFTP software.
    * Website becomes live on internet

## Why Node.js is Popular
* **1. Event-Driven**

    * Runs code when events happen.
        * Example:

            * File read completed
            * Request received
* **2. Non-Blocking I/O**

    * Node.js does not wait for one task to finish before starting another.

        * Example:

        * Can handle many users/requests at same time.

         This makes Node.js:

                * Fast
                * Efficient

* **3. Event Loop**

* Handles async tasks and callbacks.

     Flow:

        * Tasks go to queue
        * Event loop checks queue
        * Executes tasks one by one
        
* **4. npm**

* npm = Node Package Manager

* Used to install libraries/packages.

Example:
```jsx
npm install express
```
* **5. require()**

* Used to import modules/files.

Example:
```jsx
const http = require("http");
```
* **6. Modules**

* Reusable blocks of code in Node.js.

* Can use:

    * Built-in modules
    * Third-party modules
    * Own modules