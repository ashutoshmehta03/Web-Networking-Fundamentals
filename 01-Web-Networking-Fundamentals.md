# 1. HTTP (Hypertext Transfer Protocol)

HTTP is the foundational protocol of the World Wide Web. It enables the transfer of hypertext documents, images, APIs, and other resources between a client and a server. It follows a request–response model, where the client sends a request, and the server returns a corresponding response.

Key Concepts:

1. Hypertext: Text containing links (hyperlinks) that allow navigation between documents/resources.

2. Protocol: A set of rules defining how data is formatted, transmitted, and received to ensure accurate communication.

# 2. Tools to Understand HTTP/HTTPS

1. Network Tab (Browser DevTools): Shows network requests (HTML, CSS, JS, images, API calls). Useful for monitoring status codes, payload, and debugging.

2. Inspect Element: View and temporarily modify webpage HTML, CSS, and DOM elements for testing and layout debugging.

3. Page Source: Displays the raw HTML delivered by the server before client-side modifications.

# 3. HTTP Characteristics: State, Stateless, Session

1. State: Maintaining information about a client’s previous interactions.

2. Stateless: HTTP is stateless; each request is independent and must contain all necessary information.

3. Session: Server-side mechanism to maintain user-specific data across multiple requests.

# 4. Cookies and Cache

1. Cookies: Small data stored in the client browser to identify users, maintain sessions, and personalize experience.

2. Cache: Temporary storage of frequently accessed resources to improve performance and reduce server requests.

# 5. HTTP Headers

Key–value pairs sent in requests/responses providing metadata and instructions.

Important Headers:

User-Agent: Identifies browser, OS, and device.

Date/Time: Timestamp of request.

Cookie: Sends stored cookies to the server.

Content-Type: Format of request body (e.g., application/json).

Purpose: Helps servers understand client type, session info, data format, and request time.

# 6. HTTP Request Model

Components:

1. HTTP Method: GET, POST, PUT, PATCH, DELETE, HEAD, OPTIONS

2. URL / Endpoint

3. Headers – e.g., User-Agent, Cookie, Content-Type, Authorization

4. Parameters – Query or Path

5. Body / Payload – Data sent (usually JSON)

Methods Explained:

GET: Retrieve data

POST: Create new data

PUT: Replace existing data

PATCH: Partially update data

DELETE: Remove resource

HEAD: Only headers

OPTIONS: Allowed methods (CORS)

# 7. HTTP Response Codes

1. 100 – Informational: Request received, processing continues (100, 101)

2. 200 – Success: Request processed successfully (200 OK, 201 Created)

3. 300 – Redirection: Client must follow another URL (301, 302)

4. 400 – Client Error: Request error (400 Bad Request, 401 Unauthorized, 404 Not Found)

5. 500 – Server Error: Server failed to process (500 Internal Server Error)

# 8. HTTP/2 and HTTPS

HTTP/2: Improves performance using compression, multiplexing, and binary framing.

Encryption (HTTPS): Uses TLS/SSL to secure communication.

Compression: Reduces message size.

Multiplexing: Sends multiple requests/responses over one TCP connection.

# 9. TCP (Transmission Control Protocol)

Reliable, connection-oriented transport protocol ensuring ordered delivery of data.

Three-Way Handshake (Connection Setup):

1. SYN: Client → Server (initial sequence number)

2. SYN-ACK: Server → Client (acknowledges client + sends its sequence number)

3. ACK: Client → Server (acknowledges server)

# 10. UDP (User Datagram Protocol)

Connectionless protocol; sends independent packets (datagrams) without delivery guarantee.

Basic Flow:

1. Application builds datagram with payload and destination IP:port

2. UDP adds header and hands it to IP

3. Receiver gets datagram; lost or out-of-order packets are not retransmitted

4. DNS (Domain Name System)

Translates human-readable domain names to IP addresses.

Flow:

1. User enters domain → client asks recursive resolver

2. Resolver checks cache → if missing, queries root server

3. Root server → TLD server → authoritative server

4. Resolver returns IP to client and caches it

# 12. HTTP over TCP / QUIC

Traditional HTTP: Runs over TCP using the three-way handshake.

HTTP/3: Runs over QUIC (UDP-based) for low-latency web connections.

Flow:

1. TCP/QUIC connection established

2. Client sends HTTP request

3. Server responds with status code, headers, and body

4. Connection may be reused or closed

# 13. URL Structure & Components

1. Protocol: HTTP / HTTPS

2. URN: Unique resource identifier

3. Host: Domain or IP

4. Port: 80 / 443 / 8443

5. Resource Path: File or API endpoint

6. Query Parameters: Optional ?key=value

7. Network Tools: Browser network tab shows requests, responses, headers, timings

# 14. OSI Model (7 Layers)

Conceptual model to standardize network communication in 7 layers.

Layers:

1. Application Layer (7): User interface; HTTP, FTP, SMTP.

2. Presentation Layer (6): Data formatting, encryption.

3. Session Layer (5): Session management.

4. Transport Layer (4): TCP/UDP; reliability and segmentation.

5. Network Layer (3): Logical addressing and routing.

6. Data Link Layer (2): Node-to-node delivery with frames.

7. Physical Layer (1): Transmission of raw bits over medium.

Step-by-Step Flow:

1. Browser sends HTTP request (Application)

2. Request formatted and encrypted (Presentation)

3. Session established with server (Session)

4. TCP segments request (Transport)

5. IP routes packets (Network)

6. Ethernet frames sent with MAC (Data Link)

7. Bits travel through cable/wireless medium (Physical)
