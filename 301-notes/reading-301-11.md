# Reading 301-11: Authentication

## What is OAuth?
This article by Roger A. Grimes and Josh Fruhlinger is available [here](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html).

OAuth is an authentication protocol that enables services to streamline their login process by offering a standardized way to verify login credentials. The most common implementation of this one is likely to encounter are websites that allow users to login via a larger site's login services. 

The article then provides a breakdown of the interactive request process that OAuth uses to execute acquiring the desired authorizations. This process happends over a number of steps with requests at each stride. The website that is providing the authorization provides a temporary set of secret credentials to validate the login, they exchange tokens and have the user confirm the transaction, and then the user has authorized acces to the site's features. 

## Auth0 Docs: Authentication and Authorization Flows
This documentation is available [here](https://auth0.com/docs/flows).

The Auth0 docs explain that Auth0 can involve a number of flows with which to handle authorization, and provides a breakdown of several options for this: 

- Authorization Code Flow
- Authorization Code Flow w/ Proof Key for code exchange
- Implicit Flow with Form Post
- Hybrid Flow
- Client Credentials Flow
- Device Authorization Flow
- Resource Owner Password Flow

### Additional Bookmarks

[React SDK for single page apps](https://auth0.com/docs/libraries/auth0-react)


[<<Return to Home](../README.md)