# Reading 401-19: Roles, Claims, and Tokens

## Microsoft Docs: Claims-Based Auth in ASP.NET Core
This documentation is available [here]().

Once we have established identity, we can use the various claims that form an identity for authorization. This can be done with a variety of different claims, even multiple at once. 

This documentation offers examples of both pahts, from dependency injection in the configuration to adding the authorizaition annotations and permissions. 

## Andrew Lock: Intro to Claims in ASP.NET
This article is available [here]().

There are two sides of security that are dependent on each other, Authorization and Authentication. Authentication is the process of verifying who you are, whereas Authorization determines what you are allowed to do once we have ascertained your identity. 

Naturally these processes begin with Authentication, which is done via claims. We can do this by specifying an AuthenticationType that we check in order to perform the Authentication.


[<<Return to Home](../README.md)