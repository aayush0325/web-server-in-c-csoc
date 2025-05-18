# Web server in C

A web server software is a program that handles HTTP requests from clients (typically web browsers) and serves web content in response.

for systems programming track of CSoC 2025, we'll be writing an HTTP web server in C.

## Project Goals

The goal is to build a functional HTTP web server. The implementation should handle core protocols, manage client interactions, and ensure secure resource delivery. Essential capabilities include:

### Core Protocol Handling

*   Parse HTTP requests (methods like GET, POST, HEAD), including headers, query parameters, and body data.
*   Generate compliant HTTP responses with status codes (e.g., 200 OK, 404 Not Found), headers (e.g., Content-Type, Content-Length), and optional body content.
*   Support HTTP/1.1 features like persistent connections (Keep-Alive) and chunked transfer encoding.

### Resource Management

*   Serve static files (HTML, CSS, images) from a designated directory, handling MIME types and cache headers.
*   Route requests to dynamic endpoints if applicable (e.g., API endpoints or server-side scripts).
*   Handle errors gracefully, including 4xx client errors and 5xx server errors, with user-friendly messages.

### Concurrency and Performance

*   Manage multiple simultaneous connections via threading, multiprocessing, or asynchronous I/O.
*   Limit resource usage (bandwidth, memory) to prevent overload, especially under high traffic.

### Security Features

*   Sanitize input paths to prevent directory traversal attacks (e.g., blocking `../` in URLs).

## Resources

*   [csoc resources](./csoc_resources)

## Weekly Standup

Every Sunday, we'll have a standup call to discuss the project's progress, address any doubts, and plan for the upcoming week. This is a great opportunity to collaborate and ensure everyone is on the same page.

## Tasks

Familiarize yourself with the HTTP protocol and web server concepts. Set up a development environment with necessary tools (e.g., compiler, debugger).

*   [Week 1 tasks](./tasks/week1.md).
