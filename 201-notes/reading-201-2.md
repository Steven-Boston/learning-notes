# Reading 201-2
## Duckett HTML 2:Text
Chapter 2 begins with an overview of the elements used to define and contain different types of text, namely:
- `<h1>` with numbers 1-6 create different sized headings. 
- `<p>` contains paragraphs
- `<b>` and `<i>` form bold or italic text
- `<sup>` and `<sub>` make superscript and subscript
- `<br />` creates a line break
- `<hr />` creates a line divider between sections of text

There are also several types of semantic markup that create superficial but subtly important designations for particular pieces of content:
- `<strong>` and `<em>` indicate importance, and will usually be displayed in bold and italic, respectively. 
- `<blockquote>` and `<q>` are for quotations, with blockquote also usually carrying indentation by default. 
- `<abbr>` with title attribute will allow you to define the meaning of an abbreviation. 
- `<cite>` adds italics to text to help form a citation.
- `<dfn>` indicates an initial definition, and some less common browsers will render this element with italics. 
- `<address>` sections contain contact information, such as mailing or email addresses.
- `<ins>` and `<del>` indicate removed or added text, wit del granting a strikethrough and ins adding underline.
- `<s>` contains outdated information that is to remain on the page, and also confers a strikethrough. 

## Duckett HTML 10: Introducing CSS
*this section from 102.5 notes*

CSS code allows you to create rules that govern the appearance and design of each element of your webpage. 
Each rule requires a *selector* and a *declaration*. The selector describes which elements will be affected, and the declaration describes what effect will be applied to them. 
The declaration has two parts: a **property** and a **value**, which are separated by a colon. 
CSS code can be placed in another file by using `<link href="CSSlocation.example">` to make the browser reference the file. 
CSS code can also be included within the html file using `<style type="text/css">`, usually within the head. websites with multiple pages are often better served with one external CSS page that governs the entire site. 
CSS allows for comments to be added via `/*.....*/`
#### Selectors
There are many selectors available in CSS, Duckett outlines some common examples:
- Universal Selector: `* {}` targets all elements
- Type Selector: `h1, p, li, {}` targets all elements of the specified type. 
- Class Selector: `.class {}` targets the class specified after the period. 
- ID selector: `#introduction {}` targets anything with the specified id attribute
- Child Selector: `article>p {}` targets the second element when it is a child of the first. 
- Descendant Selector: `article p {}` targets the second element even when it is an inderect descendant of the first. 
- Adjacent Sibling Selector: `h2 + p {}` targets the second when it is the direct sibling of the first. 
- General Sibling Selector: `h2~p {}` targets all instances of the second that are siblings with the first. 
#### Cascading Priority & Inheritance
- Later rules will supercede earlier oens
- More specific rules will supercede less specific ones
- ` !important` added after a value will give it priority
- child elements inherit values

## Duckett Javascript 2: Basic Javascript Instruction
Javascript is formed from ordered statements that define what the computer should do. Comments can (and should) be added via `//` to add context for human eyes. For multiple lines, `/* */` can contain the comments.
Variables are the method by which the computer running the script can be asked to remember data for later use. Variables can be declared by declaring type, name, and value as in `var message = "hello world"`, and can store many different types of data. 
Once declared, a simple `varName = value` can alter the value of a variable. 
Variable names must begin with $, _, or a letter (not a number). The rest of the name can include those options as well as numbers, but cannot include keywords vital to javascript. Variable names are also case sensitive, and should use camel case inThisFormatToDelineateWords or_With_Underscores. Making variable names semantic also contributes to readable code.
### Arrays
Arrays are a type of variable that can store multiple values (generally a list). they can be created using brackets [] when manipulating the variable and separating each value with a comma in the form

`var thingsList = ['thing1', 'thing2', thing3']`

alternatively, `new Array();` can be used. Once the array is established,  you can reference a particular array item via `thingslist[0]`. Keep in mind that arrays begin at position 0. 

### Operators
*this section from reading-102.7*

**Expressions** take a value and assign it to a variable. They can do this either by defining the value straight out or combining multiple items to synthesize it. 
Expressions achieve this via **operators**, which come in several types:
- Assignment Operators directly assign a value (`color = 'blue';`)
- Comparison Operators compare values and return a boolean (`acquire = 4>3;`)
- Arithmetic Operators perform calculations (`manaValue = 3 + 2;`)
- Logical Operators Combine expressions to return a boolean (`cast = (4>3) && (5>4);`)
- String Operators combine strings (`priority = 'in ' + 'response';`)

Arithmetic has several functions available:
- Addition + and Subtraction -
- Multiplication * and Division / 
- Increment ++ and Decrement --
- Modulus % (divides values and returns remainder)
These operations folloe standard order of operations.

## Duckett Javascript 4: Decisions and Loops
Most scripts feature some level of branching paths that can be used in different situations. The computer is able to select the correct path using a **decision**, which consists of a value generated by an expression, to be analyzed via a conditional statement. 
==, !=, >, <, >=, and <= (and === and !==) allow for **comparisons**, which return a true or false value by comparing two objects. 
**logical operators** allow for the comparison of multiple comparison  operators in tandem. && checks if all items meet a condition, `||` checks if at least one item meets a condition. ! will invert an otherwise normal comparison, giving the opposite boolean. Logical operators evaluate left to right, and stop when the collected results are sufficient to make a determination.
Storing the result of an expression using a logical operator can return a boolean to be stored in a variable, or checked for if statements or while loops. 
**if statements** are created via `if (conditional statement) {} else{}`, and allow for different code to be executed (or not executed) depending on the situation as assessed via the conditional statement. 

## Chris Beams on Commit Messages
*notes on [this article](https://chris.beams.io/posts/git-commit/)*

Commit messages can help maintain a project over a large period of time and/or communicate developer intent to other people working on a project. Having a cohesive and consistent strategy for writing them will make the commit log a resource rather than a roadblock. 
### The Seven Rules for a Great Commit Message:
1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. No end punctuation on the subject line
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Focus on what changes were made and **why**

Chris also makes mention of the power of terminal commmands specific to git and their role in manipulating git's many functions, and recommends the book [Pro Git](https://git-scm.com/book/en/v2), which can be read online for free.

[<<Return to Home](../README.md)