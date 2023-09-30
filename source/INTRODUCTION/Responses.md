# 📩 Responses

---

Lucidya have applied all the technical standards have been placed by the REST principles. So, developers can always receive, read, decode, or understand the errors in responses based on the following tables.

## ✅ Successful Response Codes

COLOR CODE | RESPONSE | STATUS | Description |
---------|----------|---------|---------|
 ![green.png](../assets/green.png) | **200** | Success & OK | Successful HTTP request |
 ![green.png](../assets/green.png) | **201** | Created | API call has been accepted for processing. The sent resource has been successfully inserted/updated at our database |
![green.png](../assets/green.png) | **202** | Accepted | API call has been accepted for processing. This status code is used only when the sent resource has been successfully deleted from our database |
 ![green.png](../assets/green.png) | **204** | No Content | The server successfully processed the request, but is not returning any content |

!!! tip "💡 Note"
    With **2xx** response (success) you'll receive in response body success field denoting the success value and it will be set to true, field status The HTTP status returned and it will be (2xx), as the following example

## ❌ Error Response Codes

With every request you might get these responses in case of any error :

COLOR CODE | RESPONSE | SLUG | STATUS | Description |
---------|----------|---------|---------|---------
 ![orange.png](../assets/orange.png) | **400** | bad_request | Bad Request | Invalid parameters, fields or filters.
 ![orange.png](../assets/orange.png) | **401** | unauthorized | Unauthorized | Authorization error (Invalid API key).
 ![orange.png](../assets/orange.png) | **403** | forbidden | Forbidden | The server understood the request, but is refusing it (blocked due to many errors in particular time) or the access is not allowed.
 ![orange.png](../assets/orange.png) | **404** | not_found | Not Found | The specified resource/url-path could not be found.
 ![orange.png](../assets/orange.png) | **405** | method_not_allowed | Method Not Allowed | The method used is not allowed.
 ![orange.png](../assets/orange.png) | **406** | not_acceptable | Not Acceptable | The format used is not acceptable.
 ![orange.png](../assets/orange.png) | **410** | gone | Gone | The resource requested is no longer available.
 ![orange.png](../assets/orange.png) | **422** | validation_failed | Unprocessible Entity | Used if the server cannot process the enitity, e.g. mandatory fields are missing in the payload.
 ![orange.png](../assets/orange.png) | **429** | too_many_requests | Too Many Requests | Rate limit exceeded.
 ![red.png](../assets/red.png) | **500** | server_error | Internal Server Error | We might be updating our services, please wait a while before trying again.
 ![red.png](../assets/red.png) | **503** | service_unavailable | Service Unavailable | We were unable to handle the HTTP request due to a temporary overloading or maintenance of the server. Please try again later.
 ![red.png](../assets/red.png) | **504** | time_out | Gateway Timeout | it means the server tried to load the data or fulfill another request but it took too long and timed out.

!!! warning "⚠️ Error Response Codes"
    In case of multiple errors as the result of a request (**4xx** response), a list of "fields" and an array of messages as "values" of those fields (explaining the error in each field) will be provided. Hope the following example gives you a hint.

### 🔴 Error Message

```json
{
  "error": {
    "status": 401,
    "detail": "Failure of getting data due to monitor not found"
  }
}
```
