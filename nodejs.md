# 05. Node.js Interview Questions

## Questions

1. Explain the Node.js event loop.
2. Why is Node.js good for I/O-heavy applications?
3. When is Node.js a poor choice?
4. How do you handle CPU-intensive operations in Node.js?
5. What are Node.js streams?
6. Explain readable, writable, duplex, and transform streams.
7. How would you process a 10 GB file without loading it into memory?
8. How do you handle errors in an Express/Node.js API?
9. How would you implement centralized error handling?
10. How would you implement authentication in Node.js?
11. JWT vs session-based authentication?
12. How do you validate JWT tokens?
13. How do you handle token expiration?
14. How do you secure a Node.js API?
15. How do you prevent SQL injection, NoSQL injection, XSS, CSRF, and CORS issues?
16. How do you implement rate limiting?
17. How would you scale a Node.js application horizontally?
18. What is Node.js clustering?
19. How do you implement graceful shutdown?
20. How do you handle unhandled promise rejections?
21. How would you monitor a Node.js application in production?

## Production Scenario

> A Node.js service memory usage keeps increasing until the container is killed. How would you investigate?

Discuss:

- Heap usage and heap snapshots
- Event listeners
- Unclosed connections
- Timers
- Caches
- Large in-memory objects
- Stream handling
- Garbage collection
- Container memory limits
- Application metrics and logs
