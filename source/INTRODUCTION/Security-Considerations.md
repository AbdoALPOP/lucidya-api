# 🛡️ Security Considerations

---

The Lucidya API employs a **RESTful** architecture, offering a straightforward interface with structured responses in **JSON** format. This allows developers to harness many of Lucidya's features with ease.
This article aims to supply essential security information and considerations for developers when integrating with the Lucidya API.

## 🌐 SSL and TLS

The Lucidya system supports **SSL and TLS** cryptographic protocols which designed to **provide secure communication over a network**.
**SSL** stands for **Secure Sockets Layer**, and **TLS** stands for **Transport Layer Security**. They are most commonly used to secure web systems, and also secure other types of data transfers.

The Licidya REST APIs use **HTTP** and support **Transport Layer Security (TLS)** encryption. TLS is a standard that keeps an internet connection private and checks that the data sent between two systems (a server and a server, or a server and a client) is encrypted and unmodified.

## API

API requests must use **HTTPS**, **HTTP requests will not be allowed**. Lucidya API prevents anonymous users from accessing the APIs that could reveal sensitive information, you can have access only through your access_token that you can get from the [Lucidya settings](Authorization.md).

## 🕒 Token Expiration & Deactivation

Token expiration refers to the **period of validity for an access token**, after which it becomes invalid. When a token expires, it can no longer be used to make API calls. In order to continue making API calls, you will need to create a new token.

!!! warning "⛔️ Token Deactivated"
    If the key is not used within a **30-day** period, the token will be deactivated and you will receive an email about the deactivation for your convenience and security.

!!! warning "🗓️ Token Expiration"
    if the key is utilized continuously for a **60-day** period, the token will reach its **expiration**. An email alert will be sent to you about this expiration, ensuring your convenience and security.
