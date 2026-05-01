# Table of Contents
* [1. API Overview]([# 1. API Overview](https://github.com/astry-ec/API_Documentation_JSONPlaceHolder/blob/main/API_Documentation.md#1-api-overview))


# 1. API Overview

**Base URL:**

```text
https://jsonplaceholder.typicode.com
```

The User Data API allows external applications to retrieve user profile information from the system of **ABC Blogging Website**. It can be used by other applications to display user details, sync customer records, or validate user information.

The API returns data in JSON format and is intended for integration with web applications, reporting tools, and internal business systems.

# 2. Use Cases
- This API can be used to:
- Retrieve a list of registered users
- View detailed information for a specific user
- Support testing for user data integration

# 3. Available Endpoints

There are 6 available endpoints which serve different purpose

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | /posts   | Retrieve all user's posting |
| GET    | /comments | Retrieve all comment of user in a postin |
| GET    | /albums   | Retrieve all album |
| GET    | /photos | Retrieve all photos |
| GET    | /todos | Retrieve all user's to do list |
| GET    | /users  | Retrieve all users |


## /posts

```text
GET https://jsonplaceholder.typicode.com/posts
```
This endpoint provides data about user's posting in the website

Example data:
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
## /comments
    
```text
GET https://jsonplaceholder.typicode.com/comments
```
This endpoint provides data about user's comment from each posting available in the website

Example data:
```text
[
    {
        "postId": 1,
        "id": 1,
        "name": "id labore ex et quam laborum",
        "email": "Eliseo@gardner.biz",
        "body": "laudantium enim quasi est quidem magnam voluptate ipsam eos\ntempora quo necessitatibus\ndolor quam autem quasi\nreiciendis et nam sapiente accusantium"
    }
]
```
## /albums

```text
GET https://jsonplaceholder.typicode.com/albums
```
This endpoint provides album's title of each user id

Example data:
```text
[
    {
        "userId": 1,
        "id": 1,
        "title": "quidem molestiae enim"
    },
    {
        "userId": 1,
        "id": 2,
        "title": "sunt qui excepturi placeat culpa"
    }
]
```
## /photos

```text
GET https://jsonplaceholder.typicode.com/photos
```
This endpoint provides URL link of a photos and the album id where it is located

Example data:
```text
[
    {
        "albumId": 1,
        "id": 1,
        "title": "accusamus beatae ad facilis cum similique qui sunt",
        "url": "https://via.placeholder.com/600/92c952",
        "thumbnailUrl": "https://via.placeholder.com/150/92c952"
    },
    {
        "albumId": 1,
        "id": 2,
        "title": "reprehenderit est deserunt velit ipsam",
        "url": "https://via.placeholder.com/600/771796",
        "thumbnailUrl": "https://via.placeholder.com/150/771796"
    }
]
```
## /todos

```text
GET https://jsonplaceholder.typicode.com/todos
```
This endpoint provides to do list of each user id

Example data:
```text
[
    {
        "userId": 1,
        "id": 1,
        "title": "delectus aut autem",
        "completed": false
    },
    {
        "userId": 1,
        "id": 2,
        "title": "quis ut nam facilis et officia qui",
        "completed": false
]
```
## /users

```text
GET https://jsonplaceholder.typicode.com/users
```
This endpoint provides list of users of the website

Example data:
```text
[
    {
        "id": 1,
        "name": "Leanne Graham",
        "username": "Bret",
        "email": "Sincere@april.biz",
        "address": {
            "street": "Kulas Light",
            "suite": "Apt. 556",
            "city": "Gwenborough",
            "zipcode": "92998-3874",
            "geo": {
                "lat": "-37.3159",
                "lng": "81.1496"
            }
        },
        "phone": "1-770-736-8031 x56442",
        "website": "hildegard.org",
        "company": {
            "name": "Romaguera-Crona",
            "catchPhrase": "Multi-layered client-server neural-net",
            "bs": "harness real-time e-markets"
        }
    },
    {
        "id": 2,
        "name": "Ervin Howell",
        "username": "Antonette",
        "email": "Shanna@melissa.tv",
        "address": {
            "street": "Victor Plains",
            "suite": "Suite 879",
            "city": "Wisokyburgh",
            "zipcode": "90566-7771",
            "geo": {
                "lat": "-43.9509",
                "lng": "-34.4618"
            }
        },
        "phone": "010-692-6593 x09125",
        "website": "anastasia.net",
        "company": {
            "name": "Deckow-Crist",
            "catchPhrase": "Proactive didactic contingency",
            "bs": "synergize scalable supply-chains"
        }
    }
]
```
# 3. How to Access it
## Non-Developers

- **Access directly from a web browser**

<img width="918" height="1026" alt="image" src="https://github.com/user-attachments/assets/7ed7aa1f-35a0-4801-b085-30ff001c7c69" />

## Developers

- **Access from terminal/cmd**
```text
curl https://jsonplaceholder.typicode.com/users
```

<img width="774" height="939" alt="image" src="https://github.com/user-attachments/assets/f776f3a6-c879-4ce6-841b-a2d6fcf05e7e" />


- **Access directly from programming language**

  example from python

```text
import requests

url = "https://jsonplaceholder.typicode.com/users"
response = requests.get(url)

print(response.json())
```

- **Access from postman**

<img width="750" height="931" alt="image" src="https://github.com/user-attachments/assets/d80e293c-45cb-4a69-a60d-d9c56a0e8295" />


# 3. Limitation
