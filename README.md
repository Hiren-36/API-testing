#API Testing Collection
This Postman collection is designed for testing basic API functionalities, using Reqres.in as a mock API service. It covers essential API operations for managing users, including creating a new user and retrieving users.

#Collection Overview
Name: API Testing
Postman Collection Schema: v2.1.0

#Included Following Requests
#Create User:
Method: POST
Endpoint: https://reqres.in/api/users
Request Body:json
Payload :
{
  "name": "morpheus",
  "job": "leader"
}
Tests:
Status code should be 201
Response time should be below 10ms
Content-Type should be application/json

#Get Single User:
Method: GET
Endpoint: https://reqres.in/api/users/4
Tests:
Status code should be 200
Response time should be below 500ms
Content-Type should be application/json

#Get All Users:
Method: GET
Endpoint: https://reqres.in/api/users
Tests:
Status code should be 200
Response time should be below 500ms
Content-Type should be application/json
