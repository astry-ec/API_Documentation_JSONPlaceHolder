# 1. API Overview

**Base URL:**

```text
https://jsonplaceholder.typicode.com
```

The User Data API allows external applications to retrieve user profile information from the system. It can be used by other applications to display user details, sync customer records, or validate user information.

The API returns data in JSON format and is intended for integration with web applications, reporting tools, and internal business systems.

# 2. Use Cases
- This API can be used to:
- Retrieve a list of registered users
- View detailed information for a specific user
- Support testing for user data integration

# 3. Available Endpoints

There are 6 available endpoints which serve different purpose

## a. /posts

```text
GET https://jsonplaceholder.typicode.com/posts
```
This endpoint provides data about user posting

```text
[
    {
        "userId": 1,
        "id": 1,
        "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
        "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
    }
]
```


# How to Access it
# 3. Limitation
