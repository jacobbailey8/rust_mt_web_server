# Simple Rust Web Server with Thread Pool

This is a basic web server implemented in Rust that uses a custom-built thread pool to handle incoming TCP connections concurrently. It demonstrates key Rust concepts such as multithreading, message passing, ownership, and synchronization.

## Features

- Custom `ThreadPool` implementation using `std::thread`, `mpsc`, and `Arc<Mutex<_>>`
- Basic HTTP request parsing
- Serves different HTML files based on the request path
- Simulates long-running tasks (`/sleep` endpoint)
- Graceful shutdown of worker threads using Rust's `Drop` trait
