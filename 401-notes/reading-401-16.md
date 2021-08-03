# Reading 401-16: Refactoring with Data Transfer Objects

## Microsoft Docs: Creating Data Transfer Objects
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/part-5).

Data Transfer Objects are models for data that are specifically designed to send data out in a controlled fashion. Once established, a data transfer object will supercede the full table data when a request for that data is made and become the form in which the request is fulfilled. This entails writing the DTO as a subset of the properties of the full data set and then adjusting the services to use the model in responding. Additional details and full code examples are available in the documentation. 

## Joydip Kanjilal: Using DTOs
This article is available [here](https://www.infoworld.com/article/3562271/how-to-use-data-transfer-objects-in-aspnet-core-31.html).

Data transfer objects are useful for keeping responses to a manageable size as well as concealing the internal structures of a database. DTOs are used to manage data transfers between layers in an API, and as a result it is best if they are immutable.



[<<Return to Home](../README.md)