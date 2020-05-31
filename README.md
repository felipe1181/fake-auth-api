# JSONServer + JWT Auth

A Fake REST API using json-server with JWT authentication. 

Implemented End-points: login,register

## Install

```bash
$ npm install
$ npm run start-auth
```

## Endpoints
```
POST http://localhost:8000/auth/login
POST http://localhost:8000/auth/register
```
```
{
  "email": "felipe@email.com",
  "password":"123"
}
```

You should receive an access token with the following format 

```
{
   "access_token": "<ACCESS_TOKEN>"
}
```


You should send this authorization with any request to the protected endpoints

```
Authorization: Bearer <ACCESS_TOKEN>
```



