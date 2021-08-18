# Reading 401-18: Identity

## Microsoft Docs: Identity on ASP.NET Core
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-2.1&tabs=visual-studio).

Identity is a system in ASP.NET Core that allows the ambitious developer to incorporate login services to their applications. Logins can be handled through several third party services and stored in a database or similar info bank. 

## David McCullough: ASP.NET Authentication and Authorization Demystified
This blog post is available [here](https://digitalmccullough.com/blog/aspnetcore-auth-system-demystified/).

In this article McCullough endeavors to give an overview of authorization in asp.net core. He starts by explaining that identity has three components:

### Claims

A claim is simply a single property of a user. This can be anything from a username, some status, or email. This essentially equates to someone making a 'claim' about themselves. 

### ClaimsIdentity

A ClaimsIdentity is an object comprised of claims formatted to be used for authentication, generally with a small collection of user information that can be verified. 

### ClaimsPrincipal

A ClaimsPrincipal is an abstract representation of a user, usually comprised of multiple ClaimsIdentity's. This caps out the structure by which this data is handled in Identity.

## Identity Verbs

Next we head into the wonderful world of verbs: 

- Authenticate: retrieve the user's data
- Challenge: verify the data
- SignIn: keep a persistent record of the user
- SignOut: get rid of the signIn records
- Forbid: Rebuff unwanted users

## Auth Flow

McCullough spends the remainder of the article explaining the code components that deal with these data and actions, including an excellent flow chart that breaks down the path of the wayward ClaimsPrincipal. He also includes some sample code that models this setup. 


[<<Return to Home](../README.md)