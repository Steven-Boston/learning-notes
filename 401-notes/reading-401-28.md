# Reading 401-28: Auth/Cookies

## MDN Docs: Using HTTP Cookies
This documentation is available [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies).

Cookies are snippets of raw text that are sent to the browser by an API. Browsers are setup to send the cookie data back with subsequent requests, allowing for continuity and maintaining of data over a number of situations .

According the the documentation, cookies have three main uses: 

- Session Management
- Personalization
- Tracking

Cookies are sent with a response via a set-cookie header, which can be set when arranging the response. The cookies have a number of options that can be used when sending, including expiration, access, destinations, and others.  

## Nicholas C Zakas: HTTP Cookies Explained
This article is available [here](https://humanwhocodes.com/blog/2009/05/05/http-cookies-explained/).

Nicholas covers some of the same ground as the documentation above, but goes into additional detail on how cookies are sent and the parameters therein. This includes secions on several types of options: 

- Expires
- Domain
- Path
- Secure 

He then goes on to discuss the trials of managing cookies from the API end, including how to keep the cookies consistent and handle when they are not. This includes updating details, setting restrictions, and making choices about removal. 


[<<Return to Home](../README.md)