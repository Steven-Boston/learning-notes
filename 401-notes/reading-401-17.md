# Reading 401-17: Intro to Identity

## MDN Docs: Using HTTP cookies
This documentation is available [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies).

Cookies are small pieces of data that are sent to users to keep track of their activities. This can be a matter of their indentity, behaviors, choices, or other status info. 

Cookies can be established by having the server include `Set-Cookie` headers in the server response, which will casue the browser to store the information. This means that future requests form the browser will include the cookie, allowing the server to handle the request armed with additional information. 

The rest of this docucumentation outlines various procedures that surround the use of cookies, including giving them a lifespan, determining where they will be sent, maintaining security and more. 

## Nicholas C. Zakas: HTTP Cookies Explained
This article is available [here](https://humanwhocodes.com/blog/2009/05/05/http-cookies-explained/).

Nicholas outlines the history and purpose of cookies: small bits of text data used to identify a repeat user that the server and browser pass back and forth. He then covers the reasons one might employ the tactics mentioned in the MDN docs, from keeping the scope of cookies limited in order to rein in their footprint to using limiters to rein in their impact. 

[<<Return to Home](../README.md)
