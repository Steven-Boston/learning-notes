# Reading 301-12: Mongo and Mongoose

## Luke P. Isaac: SQL vs. NoSQL
This article is available [here](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool).

Isaac breaks down the key differences in how databases store and handle the data the hoard, in particular comparing SQL vs. NoSQL databases. This broadly comes down to the newer noSQL databases having additional features like horizontal scaleability and dynamic schema, but losing some stability and support for having that less rigid approach. 

The rest of the article gives an overview of common databases, and includes mention of the one we will be using. It seems to boast impressive speed, scalability, and useability, and stores data in documents that are similar to json files. 

## Video: SQL vs. NoSQL
This video is available [here](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

This video gives a more introductory approach to presenting databases: 

- SQL databases operate on simple SQL language, which allows for the data to be called in a predictable way. This data is stored in tables, which must be fully filled out following the prescribed schematic. These tables can be linked within the database via relative links from common values via joins operations. This warrants a lot of power in acquiring data once everything is set up. 

- NO SQL databases (like hu**mongo**usDB) store data via collections. these collections contain documents that can have an entirely differect structure. This allows for an adaptable approach that lets the developer easily adapt to changing needs, but also loses some of the ease gained by a stiff structure. 

- Both options have pros and cons that need to be considered before they are selected for a project. Knowledge of both is key in making these decisions, as either can be a huge boon for the right project. 

### Additional Bookmarks

[Mongoose API](https://mongoosejs.com/docs/api.html#Model)

[<<Return to Home](../README.md)