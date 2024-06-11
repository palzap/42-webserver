## Project Overview: Webserv

### Introduction

The **Webserv** project focuses on developing a fully functional HTTP server using C++ 98. The goal is to provide an in-depth understanding of the HTTP protocol and the core principles of web communication by constructing a server from scratch. This project is vital for gaining insights into server operations and web protocol mechanics.

---

### Key Features

1. **HTTP and HTML Integration**
   - **HTTP Protocol**: Webserv supports HTTP/1.1, handling standard web requests such as GET, POST, and DELETE. This support is crucial for understanding the fundamentals of web communication and the request-response model central to HTTP.
   - **HTML Content Delivery**: The server is capable of delivering HTML content, including static files like text and images and dynamically generated content through CGI. This capability enables the server to render web pages effectively to clients.

2. **Webserver Functionality**
   - **Request Handling**: Webserv parses incoming HTTP requests, constructing accurate responses with appropriate headers and status codes. This feature mimics the operations of popular web servers like NGINX and Apache.
   - **Response Generation**: The server supports serving static files, executing CGI scripts for dynamic content generation, and handling file uploads. This comprehensive handling provides a real-world-like server environment.
   - **Non-Blocking I/O**: Utilizing the `epoll()` function, the server ensures efficient, non-blocking I/O operations, crucial for handling multiple client connections simultaneously without performance issues. This approach improves the server's ability to manage high concurrency effectively.

3. **Configuration Management**
   - **Flexible Configuration**: The server reads settings from a configuration file, allowing customization of server behavior, including server names, error pages, and port configurations. This flexibility supports varied deployment environments.
   - **Route Handling**: Configuration includes defining routes with specific rules, such as HTTP method restrictions, redirections, and file path mappings. This flexibility simulates diverse server configurations and enhances practical understanding.

4. **Resilience and Compliance**
   - **Robust Error Handling**: Webserv incorporates default error pages and accurate HTTP status codes to manage various client requests gracefully. This ensures a robust and user-friendly experience even when errors occur.
   - **Stress Testing**: The server is designed to handle stress tests, maintaining stability and availability under heavy load. This aspect is crucial for demonstrating the server's reliability and efficiency.

5. **Platform Considerations**
   - **Cross-Platform Support**: Specific considerations for MacOS include using `fcntl()` to implement non-blocking behavior due to platform-specific variations in `write()` function implementation.

---

### Implementation Details

- **Core Components**: The project involves creating core server components in C++ 98, such as socket handling, HTTP request parsing, and file I/O operations. This offers a deep dive into low-level networking and C++ programming fundamentals.
- **Non-Blocking Architecture**: Leveraging `epoll()`, Webserv ensures non-blocking I/O operations, critical for efficiently managing multiple simultaneous connections. This method improves the server's responsiveness and scalability.
- **Error Handling**: The project emphasizes strict error handling and accurate HTTP response generation, preparing the server for real-world scenarios where robust error management is essential.

---

### Conclusion

The **Webserv** project offers a thorough exercise in building an HTTP server, encompassing core aspects of web communication, server architecture, and HTTP protocol implementation. It serves as an educational tool for understanding the inner workings of web servers and HTTP interactions.

---

### Evaluation

### First submission
08/06/2024
110%

