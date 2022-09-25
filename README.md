# ecommerce

MORE TO BE ADDED

- **SIGNUP FUNCTION API CALL (POST REQUEST)**


  https://ecommerce-backendg-gosk.herokuapp.com/users/signup
http://localhost:8000/users/signup

```json
{
  "first_name": "sankalp",
  "last_name": "kumar",
  "email": "sankalp@kumar.com",
  "password": "sankalp",
  "phone": "9876543210"
}
```

Response :"Successfully Signed Up!!"

- **LOGIN FUNCTION API CALL (POST REQUEST)**

  https://ecommerce-backendg-gosk.herokuapp.com/users/login
  http://localhost:8000/users/login

```json
{
  "email": "sankalp@kumar.com",
  "password": "sankalp"
}
```

response will be like this

```json
{
  "_id": "63305fe5b6ea07341a5aae0b",
  "first_name": "sankalp",
  "last_name": "kumar",
  "password": "$2a$14$bYvw0EreDJIOi4l78.lKz.gqWFneBsc0ibSDpotOzCkkKWP1QcVj2",
  "email": "sankalp@kumar.com",
  "phone": "9876543210",
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJFbWFpbCI6InNhbmthbHBAa3VtYXIuY29tIiwiRmlyc3RfTmFtZSI6InNhbmthbHAiLCJMYXN0X05hbWUiOiJrdW1hciIsIlVpZCI6IjYzMzA1ZmU1YjZlYTA3MzQxYTVhYWUwYiIsImV4cCI6MTY2NDIwMTEzNH0.3lvcRJkop6pAtR3DU84uoJKAABtTZDGHLo6-irgppj0",
  "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJFbWFpbCI6IiIsIkZpcnN0X05hbWUiOiIiLCJMYXN0X05hbWUiOiIiLCJVaWQiOiIiLCJleHAiOjE2NjQ3MTk0NjF9.Bx5nxZEg3Q5cH3w7oqpWMJCc4LC9hELkIDGuDOGBAQU",
  "created_at": "2022-09-25T14:04:21Z",
  "updated_at": "2022-09-25T14:04:21Z",
  "user_id": "63305fe5b6ea07341a5aae0b",
  "usercart": [],
  "address": [],
  "orders": []
}
```

- **Add Product Function (POST REQUEST)**

  https://ecommerce-backendg-gosk.herokuapp.com/admin/addproduct
  http://localhost:8000/admin/addproduct

```json
  {
    "Product_ID": "616153039f29be942bd9df92",
    "product_name": "Also",
    "price": 300,
    "rating": 10,
    "image": "1.jpg"
  }
```

Response : "Successfully added our Product Admin!!"

- **View all the Products in db GET REQUEST**
  
  https://ecommerce-backendg-gosk.herokuapp.com/users/productview
  http://localhost:8000/users/productview

Response

```json
[
  {
    "_id": "63305c3d23ed196b67252e9b",
    "product_name": "Alienware x15",
    "price": 2500,
    "rating": 10,
    "image": "alienware.jpg"
  },
  {
    "_id": "63305c8223ed196b67252e9c",
    "product_name": "Also",
    "price": 300,
    "rating": 10,
    "image": "1.jpg"
  }
]
```

- **Search Product function (GET REQUEST)**

defines the word search sorting

  https://ecommerce-backendg-gosk.herokuapp.com/users/search?name=a
http://localhost:8000/users/search?name=a

response:

```json
[
  {
    "_id": "63305c3d23ed196b67252e9b",
    "product_name": "Alienware x15",
    "price": 2500,
    "rating": 10,
    "image": "alienware.jpg"
  }
]
```
