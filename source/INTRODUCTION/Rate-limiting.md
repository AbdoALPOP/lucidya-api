# 🕒 Rate Limiting

---

At [Lucidya](https://lucidya.com/), we are committed to providing a stable and fair platform for everyone. To achieve this, we implement rate limiting on all our APIs. This helps us maintain our service's reliability and ensure all users have equal access.

## ⏳ What is Rate Limiting?

Rate limiting is a technique that controls the number of requests a client can make to our API within a certain timeframe. It's a protective measure designed to prevent overuse and ensure that our service remains available to all users at all times.

## 🛡️ Your Responsibility

As a developer, you play a crucial role in managing rate limits. We ask that you:

- **Limit Calls**: Be mindful of the number of requests your application makes to our API. Try to minimize unnecessary calls where possible.

- **Cache Results**: Store responses from our API locally rather than making repeated calls for the same information. This reduces the load on our servers and improves your app's performance.

- **Retry Requests Responsibly**: If you exceed our rate limit, your request will be denied. However, you can retry the request after a certain period. Be sure to implement a sensible retry policy to avoid hitting the rate limit repeatedly.

## 🚫 Our Rate Limits

The specific rate limits that apply to you depend on the plan you're subscribed to. Our rate limits start from **100 requests per minute**. If you exceed this limit, subsequent requests will be denied until the start of the next minute.

!!! tip "💡 Remember"
    Rate limiting is there to ensure a fair and reliable service for everyone. By respecting these limits, you help us provide a better experience for all our users. If you have any questions or need further clarification on our rate limiting policies, feel free to contact our support team.

## 📧 Having trouble ?

Please don't hesitate to contact us using the support methods here:

✉️ [Support](mailto:customer.support@lucidya.com)
