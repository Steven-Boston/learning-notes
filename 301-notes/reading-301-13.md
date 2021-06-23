# Reading notes 301-13: CRUD

## Kay Ploesser: Status Codes for CRUD
This article is available [here](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/).

Status codes are numbers between 100 and 600 that can be used for http responses in order to succinctly communicate the result of the request. The first digit indicates a general category: 

- 100-199: These codes are informative, and carry a message.
- 200-299: The 200s are indicators that a request was successfull. This can have varying degrees.
- 300-399: 300s indicate redirection, meaning that the information you are seeking is somewhere else. 
- 400-499: These are errors in the client, usually an problem with a request.
- 500-599: And finally, 500s are errors from the server. 

CRUD stands for Create, Read, Update, Delete, which covers most of what APIs do. There are various error codes that are usually linked to each of these: 

- Create:
  * 200 OK
  * 201 Created
  * 202 Accepted
  * 303 See Other

- Read:
  * 200 OK
  * 206 Partial Content
  * 300 Multiple Choices
  * 308 Permanent Redirect
  * 304 Not Modified
  * 307 Temporary Redirect

- Update:
  * 200 OK
  * 204 No Content
  * 202 Accepted

- Delete:
  * 200 OK
  * 204 No Content
  * 202 Accepted

- Errors:
  * 404 Not Found
  * 405 Method Not Allowed
  * 501 Not Implemented
  * 406 Not Acceptable
  * 410 Gone
  * 414 Request URI too Long
  * 308 Permanent Redirect
  * 307 Temporary REdirect

- Permissions: 
  * 401 Unauthorized
  * 403 Forbidden
  * 404 Not Found

The article has more details about each of these cases. Sending the right error code can be a huge boon to the useability of an API. 

### Additional Bookmarks

[Building REST API with Node, Express, & Mongo](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)


[<<Return to Home](../README.md)