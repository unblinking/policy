# JSON  

## Responses  

As a basic guide, use JSend. [JSend](http://labs.omniti.com/labs/jsend) is a specification that lays down some rules for how JSON responses from web servers should be formatted.  

Example response sent from Nodejs:  
```Node
{
    status: "success",
    message: "User registered successfully.",
    data: {
        username: req.body.username
    }
}
```

Example response received by Postman:  
```JSON
{
  "status": "error",
  "message": {
    "name": "UserExistsError",
    "message": "A user with the given username is already registered"
  }
}
```
