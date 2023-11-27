# HTTP-CRUD-Operations

## Hypertext Transfer Protocol

HTTP is the foundation of any data exchange on the Web. It is a protocol used for transmitting hypermedia documents (such as HTML).
It is an application layer protocol designed with in the framework of the Internet Protocol Suite.

### 1. Request-Response Cycles:
* Clients (eg. web browsers) send HTTP requests to servers.
* Servers respond to these requests

### 2. HTTP Methods:
* **GET:** Used to rquest data from a specified resource.
* **POST:** Used to submite data to be processed to a specified resource.
* **PUT:** Used to update a resource.
* **DELETE:** Used to delete a resource.

### 3. Status Codes:
* HTTP responses include status codes indicating the outcome of the request.
* Examples: 200 (OK), 201 (Created), 400 (Bad Request), 404 (Not Found), 500 (Internal Server Error), etc.

## CRUD Operations (Create, Update, Update, Delete)

CRUD represents the four basic operations that can be performed on data:

### 1. Create (POST):
* Use the **POST** method to create a new resource on the server.
* Example:
> POST /api/users
> Content-Type: application/json
>
> {
>    "username": "jerby",
>    "email": "jerby&gmail.com"
> }

### 2. Read (GET):
* Use the **GET** method to retrieve data from a specified resource.
* Example:
> GET /api/users/123

### 3. Update (PUT or PATCH):
* Use the **PUT** method to update a resource with a new representation.
* Use the **PATCH** method to apply partial modifications to a resource.
* Example:
> PUT /api/users/123
> Content-Type: application/json
> 
> {
> "username": "new_username",
> "email": "new_email&gmail.com"    
> }

### 4. Delete (DELETE):
* Use the **DELETE** method to request the removal of a resource.
* Example:
> DELETE /api/users/123