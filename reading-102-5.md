# Coding with CSS

## Duckett 10: Coding with CSS
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

## Duckett 11: Color
Color in CSS can be applied to various elements. It can be specified in a few different ways: 
- RGB values in the form of `{color: rgb(100.100.100);}` 
- Hex Codes `{color: #ee3e80;}`
- Color names `{color: DarlCyan;}`
- `{background-color:` can be used to specify a section o f background color rather than the element itself
Contrast between foreground and background are critical for readability. `{opacity: 0.9;}` with the value between 0.0 and 1.0 will set opacity. 
CSS3 allows for HSL (hue, saturation, lightness) codes to identify colors in the form `: hsla(0,75%,95%,0.3)`, with the fourth value (a) being transparency. 



[<<Return to Home](README.md)
