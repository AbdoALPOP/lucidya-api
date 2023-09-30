# 🔢 Pagination

---

All paginated responses will append the following pagination section to the response like so:

```json
{
  “page_number”: “2",
  “count”: 113
}
```

## 🔽 Endpoints Support Pagination

By default, the API will return the results in **batch**. The `page_number` parameter may be used to increase the number of results per request.

To get the next batch of results, call the same route again with a `page_id` + 1 to the `page_number [current_page_id]` and `count [total_number_of_pages]` property received in the last call on the pagination part of the response.

!!! tip "💡 Batch Note"
    The endpoints are designed to support pagination, returning a manageable batch of **10 results per page**.

if you want to move to the pages in the [Monitors List](https://lucdya.stoplight.io/docs/lucidya-api-1/branches/main/u5xrji2z8fd86-public-api-monitors-list) endpoint, simply execute the following cURL request:

```json
curl --request GET \
  --url 'https://api.lucidya.com/monitors_list?page_id=1' \
  --header 'luc-authorization: <YOUR_ACCESS_TOKEN>'
```
