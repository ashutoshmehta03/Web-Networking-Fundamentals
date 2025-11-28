# 1. HTTP (Hypertext Transfer Protocol)

HTTP is the foundational protocol of the World Wide Web. It enables the transfer of hypertext documents, images, APIs, and other resources between a client and a server. It follows a request–response model, where the client sends a request, and the server returns a corresponding response.

Key Concepts:

1. Hypertext - Text containing links (hyperlinks) allowing navigation from one document/resource to another. It enables non-linear information flow across web pages.

2. Protocol A set of rules and standards that define how data is formatted, transmitted, and received. Ensures accurate communication between devices.

# 2. Tools to Understand HTTP/HTTPS

1. Network Tab - Browser developer tools show all network requests (HTML, CSS, JS, images, API calls). Useful for monitoring status codes, timings, payload size, and debugging.

2. Inspect Element - Allows developers to view, analyze, and temporarily modify webpage HTML, CSS, and DOM elements in real-time. Useful for UI debugging and layout testing.

3. Page Source - Displays the raw HTML code delivered by the server before client-side modifications. Provides a static view of the initial webpage structure.

# 3. State, Stateless, and Session

1. State - A system maintains information about a client’s previous interactions.
2. Stateless - HTTP is stateless; each request is independent and contains all necessary data.

3. Session - Server-side mechanism to maintain user-specific data across multiple requests (e.g., login status).

# 4. Cookies and Cache

1. Cookies - Small data stored in the client browser to identify users, maintain sessions, and personalize experience.

2. Cache - Temporary storage of frequently accessed resources to improve performance and reduce server requests.

# 5. HTTP Headers

HTTP headers are key–value pairs sent in requests/responses to provide extra information.

Important headers include:

1. Client Header / User-Agent: Identifies the client, browser, OS, and device.

2. Browser Info Header: Helps the server send compatible content.

3. Date / Time Header: Timestamp of the request.

4. Cookie Header: Sends stored cookies to the server.

5. Content-Type: Indicates the format of request body (e.g., application/json).

Headers help the server understand:

1. Who is making the request

2. What data format is expected

3. Browser capabilities

4. Session management

5. Request time

# 6. HTTP Request Model

Request Model defines the structure of data sent by the client. Ensures valid, consistent input.

Components:

1. HTTP Method: GET, POST, PUT, PATCH, DELETE, HEAD, OPTIONS

2. URL / Endpoint

3. Headers: User-Agent, Cookie, Content-Type, Authorization

4. Parameters: Query or Path

5. Body/Payload: Data sent (usually JSON)

HTTP Methods Explained:

1. GET: Retrieve data

2. POST: Create new data

3. PUT: Replace existing data

4. PATCH: Partially update data

5. DELETE: Remove resource

6. HEAD: Only headers

7. OPTIONS: Allowed methods (CORS)

# 7. HTTP Response Codes

1. 100 – Informational: Request received, processing continues (100, 101)
2. 200 – Success: Request processed successfully (200 OK, 201 Created, 204 No Content)
3. 300 – Redirection: Client must follow another URL (301, 302, 304)
4. 400 – Client Error: Request error (400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found, 405 Method Not Allowed)
5. 500 – Server Error: Server failed to process (500 Internal Server Error, 502 Bad Gateway, 503 Service Unavailable)

# 8. HTTP/2

- HTTP/2 improves web speed and performance using compression, multiplexing, and binary framing.

- HTTP/1.1 is text-based, single request per connection (fallback).

- Compression - Reduces size of messages.

- Multiplexing - Sends multiple requests/responses over a single TCP connection simultaneously.

- Encryption (HTTPS) - Secures communication using TLS/SSL.

# 9. User-Agent

The User-Agent string identifies browser, device, OS, and rendering engine for the server to customize responses.

# 10. Networking Terms

Ashutosh, [11/27/2025 2:19 PM]

1. TCP - (Transmission Control Protocol): Reliable, connection-oriented protocol for ordered packet delivery. HTTP runs on TCP.

2. FTP - Protocol for file upload/download between client and server.

3. IP (Internet Protocol) - Routes data with unique IP addresses.

4. URL (Uniform Resource Locator) - Address of a resource (protocol + domain + path + optional parameters).

5. DNS (Domain Name System) - Converts domain names to IP addresses.

6. Headers - Metadata for HTTP request/response.

7. Payload - Main data in HTTP body.

8. Cache - Temporarily stores fetched resources to optimize performance.

# 11. TCP Connection Steps (Three-Way Handshake)

1. SYN - Client → Server (initial sequence number)

1. SYN-ACK - Server → Client (acknowledges client + sends server sequence)

1. ACK - Client → Server (acknowledges server)

Result - Reliable connection established, ready for data transfer.

# 12. TLS Certificate Exchange

1. Server Sends Certificate: Contains public key, domain, CA signature, validity

2. Client Validates: Checks trusted CA, domain, expiry, and tampering

3. Optional Client Certificate: Used in mutual TLS (mTLS)

4. Secure Channel Setup: Shared encryption keys established for HTTPS

5. Importance: Prevents MITM attacks, ensures identity, privacy, and integrity.

# 13. HTTP Request Format

Structure:

1. Request Line: METHOD /path HTTP/1.1
   Example: GET /products/list HTTP/1.1

2. Headers:

- Date: Timestamp

- Host: Domain

- User-Agent: Client info

- Cookie: Session info

- Content-Type: Format of request body

3. Body (Optional) - For POST/PUT/PATCH

- { "name": "John", "age": 22 }

Full Example:

GET /api/products HTTP/1.1

Host: www.example.com

Date: Tue, 26 Nov 2025 12:30:40 GMT

User-Agent: Mozilla/5.0

Cookie: sessionId=abc123

Accept: application/json

# 14. HTTP Request/Response Process

1. Gets the response back: Server responds after client request

1. Status code: Shows result (200, 404, 500)

1. Data (Image, CSV, Text): Response body contains content

1. TCP connection closed: Connection ends; HTTP remains stateless

1. Stateless: Each request is independent; sessions/cookies handle state

# 15. URL Structure & Components

1. Protocol: HTTP/HTTPS

2. URN: Unique resource identifier (not location)

3. Host: Domain/IP

4. Connection Port: 80/443/8443 (usually hidden)

5. Resource Path: File/API endpoint

6. Query: Optional data after ?

7. Params: Mandatory route identifiers

8. Network Tab: Shows requests/responses, status, headers, timings
