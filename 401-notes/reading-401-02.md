# Reading 401-02: Unit Tests and Documentation

## You Still Don't Know How to do Unit Testing
This article by Erik Dietrich is available [here](https://stackify.com/unit-testing-basics-best-practices/).

This article gives a broad overview of best practices in writing unit tests for C#, starting with some basic ideas about what a unit test is: 

- it does not interact with the surrounding enviroment of the tested code.
- it applies scenarios specifically to test functionality, not randomly in order to stress test or get aggregate data.
- it tests a specific portion of the codebase. One might be inclined to say it tests a single *unit* of the code. Or maybe a method.

We then head into a breakdown of unit testing with simple adding method as an example. One option is to write an entire project file with a method that references and tests the target method, but that feels rather pedestrian. Instead we can turn to a testing framework. Some context clues imply that we will be using xUnit for our class operations. 

### Arrange, Act, Assert

These three delightfully alliterative words form the backbone of a good unit test. 

- Arrange all of the objects and variables that are required for testing
- Act out the actions of the test within the test code
- Assert that reality exists as you expect. An unsettling proposition. 

Following this are several other tips: 

- one assert per test. 
- each test should operate independently
- keep the tests clear and concise
- If test setup is messy, so is your code. 
- Integrate the tests as a build requirement.

## xUnit Docs
The provided link was broken, but I believe I have tracked the xUnit docs down. Far too broad to write meaningful notes on, but those docs are [here](https://xunit.net/docs/getting-started/netcore/visual-studio).

## The Art of README
This *ahem* README is available [here](https://github.com/hackergrrl/art-of-readme). In a bunch of languages. Neat!

The article begins by speculating on the history of the term README and explaining the importance and value such a document has to its creator and their customers (who are often not different entities). In short, the README is often the only opportunity the developer has to explain and promote their creation. Given this basic fact, the details and trajectory of a README suddenly seem imperative to define. You would be shocked to learn that the article puts forth its idea of these objectives, which I have generously contributed some alliteration to: 

- Explain
- Expose
- Empower
- Elaborate

These goals outline everything your README must communicate: Why do I want to use your creation? What does it do? How do I use it? Is there anything else I need to know? Keeping the word count reined in is critical, but so are the details. The remainder of the article gets somewhat granular, but it shares an excellent quote that I will include here: 

> Your documentation is complete when someone can use your module without ever having to look at its code. This is very important. This makes it possible for you to separate your module's documented interface from its internal implementation (guts). This is good because it means that you are free to change the module's internals as long as the interface remains the same.
>
>Remember: the documentation, not the code, defines what a module does. -- Ken Williams

## README best practices
This is a README template, intended to be used as such. It provides some ideas that generally agree with the above article, and is available [here](https://github.com/jehna/readme-best-practices).


[<<Return to Home](../README.md)