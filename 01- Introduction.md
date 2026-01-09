### What is the Web?

The Web (World Wide Web) is a system of interconnected web pages and web applications that are accessed over the internet using a web browser and standard protocols like HTTP or HTTPS.

### In Web: What is Client-Side and Server-Side?

- Client-Side:
  Client-side refers to the part of a web application that runs in the user’s browser and is responsible for the user interface and interactions.

- Server-Side:
  Server-side refers to the part of a web application that runs on the server and handles data processing, business logic, and database operations.

### What is HTTP?

HTTP (HyperText Transfer Protocol) is a protocol used to transfer data between a client and a server over the internet.

- Hypertext:
  Hypertext is text that contains links that allow users to move from one web page to another.

- Protocol:
  A protocol is a set of rules that defines how data is communicated between devices on a network.

#### HTTP (Human-Readable):

HTTP is a human-readable protocol, meaning its requests and responses are written in a text-based format that developers can easily read, inspect, and debug.

- Network Tab Visibility:
  Network Tab Visibility allows developers to see all HTTP requests and responses exchanged between the browser and the server, including headers, status codes, and data.

- Inspect Element:
  Inspect Element is a browser tool that lets developers view and analyze the HTML, CSS, and JavaScript received through HTTP to understand how a web page is built and behaves.

- Page Source:
  Page Source displays the raw HTML code sent by the server in an HTTP response, showing the original structure of the web page.

### What is a stateless protocol?

A stateless protocol is a communication protocol in which each request is processed independently, and the server does not store any information about previous requests made by the client.

### What is a session?

A session is a server-side mechanism used to store and maintain user information across multiple requests during a specific period of interaction with a web application.

### What is a cookie?

A cookie is a small piece of data stored in the user’s browser by a website to remember information such as login status, preferences, or user activity across multiple requests.

### What are HTTP headers?

HTTP headers are key–value pairs sent with HTTP requests and responses that carry metadata about the request, the response, or the data being transferred between a browser (client) and a server.

#### Important HTTP client headers:

- Host:
  Specifies the domain name of the server being requested.

- User-Agent:
  Identifies the browser, operating system, and device making the request.

- Accept:
  Tells the server what type of content the browser can receive (HTML, JSON, images, etc.).

- Accept-Language:
  Indicates the preferred language of the user.

- Accept-Encoding:
  Specifies supported compression methods (gzip, br).

- Authorization:
  Sends authentication credentials from the browser to the server.

- Referer:
  Shows the page from which the request originated.

- Date:
  Represents the date and time when the request was sent.

- Cookie:
  Sends stored cookies from the browser to the server to maintain session and user state

### What is the request–response model?

The request–response model is a communication mechanism in which a client sends a request to a server, and the server processes the request and returns a response with the requested data or result.

#### Important HTTP Request–Response Methods

1.  GET (Read Data):
    The client sends a request to retrieve data from the server.The server responds with the requested data.

    Common Response Codes:

    1. 200 OK – Request successful
    2. 304 Not Modified – Cached data used
    3. 404 Not Found – Resource not available

2.  POST (Create Data):
    The client sends data to the server to create a new resource.The server processes the data and confirms creation.

    Common Response Codes:

    1. 201 Created – Resource created successfully
    2. 400 Bad Request – Invalid data sent
    3. 409 Conflict – Resource already exists

3.  PUT (Update Full Data):
    The client requests a complete update of an existing resource. The server updates the resource and sends confirmation.

    Common Response Codes:

    1. 200 OK – Update successful
    2. 204 No Content – Updated, no response body
    3. 404 Not Found – Resource not found

4.  PATCH (Update Partial Data):
    The client requests partial modification of a resource. The server applies the changes and responds with success.

    Common Response Codes:

    1. 200 OK – Partial update successful
    2. 400 Bad Request – Invalid update data

5.  DELETE (Remove Data):
    The client requests deletion of a resource.
    The server deletes the resource and confirms the action.

    Common Response Codes:

    1. 200 OK – Deleted successfully
    2. 204 No Content – Deleted, no response body
    3. 404 Not Found – Resource not found
