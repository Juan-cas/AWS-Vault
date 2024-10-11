

### SSL

 Or Secure Socket Layer, is an encryption-based internet security protocol, it was first developed by Netscape in 1995 for the purpose of ensuring privacy, authentication, and data integrity in Internet communications. SSL is the predecessor of the modern TLS encryption used today.

A website that implements SSL/TLS has "HTTPS" in its URL instad of "HTTP".

![HTTP vs HTTPS](https://www.cloudflare.com/img/learning/security/glossary/what-is-ssl/http-vs-https.svg)


### How does SSL/TLS work?

- In order to provide a high degree of [privacy](https://www.cloudflare.com/learning/privacy/what-is-data-privacy/), SSL encrypts data that is transmitted across the web. This means that anyone who tries to intercept this data will only see a garbled mix of characters that is nearly impossible to decrypt.

- SSL initiates an authentication process called a [handshake](https://www.cloudflare.com/learning/ssl/what-happens-in-a-tls-handshake/) between two communicating devices to ensure that both devices are really who they claim to be.

- SSL also digitally signs data in order to provide **Data Integrity**, verifying that the data is not tampered with before reaching its intended recipient.



Resources:

[CloudFlare what is SSL/TLS](https://www.cloudflare.com/learning/ssl/what-is-ssl/)