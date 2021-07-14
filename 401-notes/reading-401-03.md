# Reading 401-03: File Manipulation / System.IO

## Microsoft Docs: File and Stream I/O
This documentation is available [here](https://docs.microsoft.com/en-us/dotnet/standard/io/).

System.IO is a vast namespace in .NET with a variety of applications related to file manupulation. These come in several categories:

- Streams
- Readers/Writers
- Async Ops
- Compression
- Isolated Storage

each of the above has a small selection of available types that can achieve most of the tasks surrounding it. 

## How to: Write to File
This tutorial is available [here](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file).

## How to: Read and Write to a new file
This tutorial is available [here](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file).

Each of the above tutorials has detailed examples of uses that live within System.IO. Some quick hits on a few details I noticed:

- `using System.IO` is the base import for all IO operations
- Most of the tools contained with in will need to be instanced. 
- Streams can be a useful multidirectional tool for manipulating text documents. 

