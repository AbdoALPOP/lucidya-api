# 🚀 Get Started

---

Lucidya APIs is a public RESTful endpoints, purpose-built for secure, fast, and easy access to social Listening data. By leveraging this API, users can access and utilize various features, such as **monitoring data** from all monitor types (Twitter, Instagram, Intercom, ...), applying filters, setting up alerts, and retrieving API usage information.

These endpoints include a suite range of APIs for:

EndPoint | Description
---------|----------
 **Monitors List** | User can access the list of all monitors data
 **Widgets** | User can select and configure widgets to suite their specific monitoring requirements.
 **Filters** | User can apply filters for specific monitoring requirements.
 **Pages** | User can select and configure widgets to suite their specific monitoring requirements.
 **Facebook Widget** | Users can access data for specific page.
 **Instagram Widget** | Users can access data and apply filters from the Instagram data source.
 **Twitter Widget** | Users can access data and apply filters from the Twitter data source.

## 🔍 What is Lucidya API?

Lucidya is a sophisticated AI-powered product designed to analyze social media data and provide businesses with valuable insights. The API allows developers to interact with the platform, enabling them to integrate its functionality into their own applications.

## 💡 Why Use Lucidya API?

The Lucidya API stands out due to its focus on providing real-time data from millions of people, offering demographic qualifications that can help businesses tailor their services effectively. It's a powerful AI SaaS product for market research and customer experience management.

## 💻 Requirements

In order to make developers' interactions with Lucidya APIs easier, and for a more seamless, professional experience, the bare minimum requirements are as follows:

1. Basic understanding of programming, API consumption, webhooks calling, and JSON schema.
2. Authentication & Authorization using the API Key.
3. Verified Lucidya Account.

## 🔌 Registering for Lucidya API

To use the Lucidya API, you need first to register on [Lucidya](https://lucidya.com/request-demo/?lang=ar). Following your registration, you'll need to get in touch with your assigned customer support manager who can assist you in enabling API access for your account. This step is crucial as it allows you to integrate Lucidya's powerful social media analytics into your own applications or systems.

## 📤 Making Your First Request

After obtaining your API key, you can make your first request to the Lucidya API by sending an HTTP request to the API's endpoint, along with your API key for authentication.

```curl
  --request GET \
  --url 'https://api.lucidya.com/monitors_list?page_id=1' \
  --header 'luc-authorization: add_your_token_here'
```

<!-- To Add the Postman Collection URL -->

<!-- 
## 🕹 Test It Out
To get going quickly, we recommend using an API collaboration tool called [Postman](https://www.postman.com/). You can use the link below to import our collection of endpoints.

[![button.svg](../../assets/images/button.svg)](https://interstellar-robot-828285.postman.co/workspace/My-Workspace~4d5d49b4-6be4-4b19-8e00-86ad83ded846/collection/25244284-c789bda3-46f6-4566-b41c-1ddb04a14a0e?action=share&creator=25244284) 
-->

## 📥 Understanding the Response

When you make a request to the Lucidya API, it will return a [response](INTRODUCTION/Responses.md) containing the data you requested. This data is usually returned in **JSON** format, which is easy to work with in most programming languages.

## 🔗 Webhooks

Webhooks are an automated way for a server to talk to another server, allowing application developers to perform actions based on certain events. They provide an efficient and secure means of receiving near-real-time notifications from other services like alerts feature. Lucidya provides [webhook to **receive alerts**](WEBHOOKS/Get-started.md).

## 🚫 Rate Limiting

Like many APIs, Lucidya implements rate limiting to ensure fair usage and maintain service stability. This means there's a limit to the number of requests you can make in a given timeframe. Be sure to check the [rate limiting](INTRODUCTION/Rate-limiting.md) for details on these limits, and design your application to handle rate limiting gracefully.

## 👏 Conclusion

The Lucidya API offers a powerful way to tap into the wealth of data available on social media. Whether you're looking to enhance your market research efforts or improve your customer experience management, this API can provide the insights you need.
