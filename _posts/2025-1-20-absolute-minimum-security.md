---
layout: post
title: 'The Absolute Minimum Every Python Web Application Developer Must Know About Security'
---

![Python Web Application Security]({{ site.baseurl }}/images/osi-security.png)

The [Open Source Initiative (OST)](https://opensource.net/) is the authority that defines Open Source. They've published my guide to security for Python web applications as a three part series. *"The Absolute Minimum Every Python Web Application Developer Must Know About Security".

Never store passwords in plain text. At a minimum you should be storing salted hashed passwords (which is probably what went wrong in the image here), even better use a key derivation function, but best of all delegate password management to a modern framework and keep it up to date. And never implement your own cryptography algorithms.

Data should be encrypted in transit and at rest. Just stealing your database shouldn't reveal sensitive information because data is encrypted at rest. You can do this with the StringEncryptedType for SQLAlchemy for example. mTLS (Mutual TLS) is how we can keep data encrypted in transit, even on our internal networks. Just getting access to your network shouldn't reveal any sensitive information because data is encrypted in transit.

These are just a few of the principles from a Defence in Depth, multi-layered, approach to security which is the approach explored in this article series:

* [Essential Python Web Security](https://opensource.net/essential-python-web-security/ )

  The Defence in Depth approach, important security principles, The OWASP Top Ten, the CVE warning system, authentication controls and security tooling.

* [Security and cryptography algorithms: A guide](https://opensource.net/security-cryptography-algorithms-python/)

  Cryptography algorithms, using the cryptography library and the Python standard library. Hashing, encryption, key exchange protocols and public/private key signature algorithms with their use cases.

* [TLS and Networking](https://opensource.net/tls-and-networking/)

  Much of our security is network security and much of that comes from TLS. We now understand all the crypto algorithms that make up TLS as a security system and can understand when, how and why to use TLS. We'll also look at the request->response cycle of HTTP, the abstraction layer developers work at, and the security issues around networking. From firewalls to cookies via LANs and sockets.

(Being able to talk about the Blowfish Cipher and the Diffie-Hellmann Elliptic Curve Key Exchange Protocol is cyberpunk, so these articles are teaching real life skills.)

Thanks to Dr David Cassandra Mertz and PyDanny (Daniel Greenfeld) for improving these articles through technical review and to Nick Vidal (and volunteers) from the OSI for their work editting and formatting the articles.
