# Reading 401-09: LINQ

## Microsoft Docs: Language Integrated Query (LINQ)
This document is available [here](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/).

The purpose of LINQ is to provide a standardized method for querying a data from a variety of sources within C#. This allows for consistent and easy writing, and speeds along the process of acquiring data.

LINQ queries return the colelcted data as IEnumerables, and will function with any dataset that supports them. 


## Microsoft Docs: LINQ Query Operations
This document is available [here]().

The aforementioned document is a breakdown of the process of querying data and tyhe various options in that space: 

- Filtering
  * comes in the form `From`, `Where`, and `Select`. Returns a subset of the data informed by the three statements.  
- Ordering
  * adding `orderby` to the above returns the dataset with an ordering that you specify. [read this](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/orderby-clause).
- Grouping
  * use the `group` clause to make your query return a list of lists via some grouping condition. Spooky. 
- Joining
  * Use `join` clause to create connections between different lists based on some pattern.
- Selecting
  * `Select` allows for the transformation of the query results via a lambda statement. 

## Microsoft Docs: Writing Queries in C#
This document is available [here]().

This document is a step by step guide on writing LINQ queries. The details are best read there, but the broad steps are:

1. Secure a data source
2. Create a query
3. Execute and test the query
4. Make changes and test further

[<<Return to Home](../README.md)