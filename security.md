---
layout: page
title: Secure Python Web Application Development
permalink: /security/
---

Security breaches can devastate organisations, compromise user data, and destroy trust. As web applications become increasingly central to business operations, secure development practices are not optional – they're essential. This intensive two day courses equips Python developers with both the theoretical understanding and practical skills needed to build secure web applications. From cryptographic fundamentals to real-world implementation patterns, you'll learn how to identify vulnerabilities and implement robust security measures at every layer of your application with a Defence in Depth approach.

The course covers important security principles, and mitigating specific vulnerabilities including The OWASP Top Ten, but is focused on secure Python web application development.

This is a practical and hands on, two day, course. Learn how to use the security tools that come in the Python standard library. Modules covered include:

* hashlib
* hmac
* secrets
* random
* socket
* ssl

Web application frameworks:

* Security features in web application frameworks for API servers and web applications
* How to secure data in Django, Flask and other popular web application frameworks
* Secure deployment practises with containers and application servers (WSGI or ASGI)

Third party libraries for cryptography and secure network access:

* authlib
* cryptography
* httpx and requests
* websocket
* jwt
* OpenZiti for application level zero trust architecture
* certifi for TLS certification verification

Tooling for secure Python development and as part of your CI pipelines:

* uv/pipenv
* pip-audit
* bandit
* ruff
* mypy
* dependabot/renovate
* Security testing

Network security with TLS:

* How, why and when to use TLS
* How TLS works
* mTLS for enhanced security
* Generating self-signed certificates for local development, with the cryptography library

Michael Foord has been a Python application developer for over twenty years, is a Python core developer and the creator of unittest.mock, and is the author of "The Absolute Minimum Every Python Web Application Developer Must Know About Security".

## Topics Covered:

### Core Python Security Fundamentals

* Security principles and defence in depth strategies with Python frameworks
* Implementing OWASP Top 10 protections in Django, Flask and FastAPI applications
* Security principles and defence in depth strategies
* Principles from The OWASP Web Security Testing Guide
* Threat modelling and the security requirements document
* The principles of least privilege and deny by default
* Zero trust architecture fundamentals
* Building zero trust architecture with OpenZiti's Python SDK

### Cryptography and Data Security

* Hashing, encryption, and digital signatures
* Symmetric encryption and public key encryption
* Secure password storage and management
* Using Python's hashlib and hmac modules for secure hashing
* Using Python's cryptography libraries correctly
* Data encryption at rest and in transit
* Data encryption at rest using Django's encrypted model fields and SQLAlchemy StringEncryptedType

### Authentication and Authorization

* Secure session management
* OAuth 2.0 and JWT for authentication
* Oauth2 with the Python library authlib
* JWT handling with PyJWT and managing token lifecycles
* Role-based access control (RBAC), plus alternatives
* Multi-factor authentication
* Managing access tokens and permissions

### Secure Coding Practices

* Proven security with modern cryptography algorithms
* Protection against SQL injection
* Input validation and sanitisation
* Using secrets vs random for cryptographic operations
* Sanitizing logs in Python applications
* Django template escaping and Flask/Jinja2 for XSS prevention
* Preventing timing attacks and token prediction attacks
* Cryptographically secure randomness
* Cross-site scripting (XSS) prevention
* Cross-site request forgery (CSRF) protection
* Secure file handling and upload validation
* Preventing TLS downgrade attacks

### Network Security

* Networking fundamentals
* TLS/SSL implementation and certificate management
* Secure API design and implementation
* WebSocket security
* Network architecture and segmentation
* Firewalls, routers, network interfaces
* Protocols, HTTP & TLS, with the Python standard library
* Application deployment
* Software Defined Networking

### Infrastructure Security

* Container security best practices
* Secure deployment patterns
* Network interfaces and routing
* Building DMZ architectures for Python web applications
* Virtual private networks (VPN)

### Security Tools and Testing

* Static analysis with bandit and ruff
* Dependency scanning using pip-audit
* Automated security testing integration
* Container scanning and runtime protection
* Code review practices for security

### Operational Security

* Live security alerts
* Statutory duties around security
* Monitoring Python applications for security issues
* Security patch management for Python applications
* Updating and patching strategies

The course includes practical exercises throughout, with participants implementing secure coding patterns, identifying vulnerabilities in sample code, and building secure components.
