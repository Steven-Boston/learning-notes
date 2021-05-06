# Reading 201-4: Links, Functions, and Layout
## Duckett HTML/CSS 4: Links
links in HTML are placed within "a" tags:

 `<a href='https://steven-boston.github.io/about-me/'>these words are a link</a>`

Clear link text is a critical detail of writing links, as only the text with the link gives much indication of where the link will go. External links require the **absolute URL** in the href attribute in order to function, where another page on the same site simply requires the file extension, or **relative URL** 

#### Directory Structure
The main folder of a website is called the **Root**, and cleanly organizing files from there is critical, especially on larger projects. The main index.html page must remain in the root, but files for JavaScript, CSS, and other pages on the site and more should be stored in folders with clear labels so that everything is easier to find. 
`<a href='mailto:steven@sample.com'>Email Steven!</a>` creates a link that opens email and begins an email to the attached address. Adding `target="_blank"` after the href attribute makes the link open on a fresh window. 
`<a href="#elementId"> will link to a specified element on the same page. The same can be added into an external link if desired to achieve the same effect. 

## Duckett HTML/CSS 15: Layout
This chapter concerns itself with the thorny business of layout in CSS, from basic positioning of different elements all the way to different overall design strategies. 

Boxes are either **block-level** or **inline**. A box within another is said to contained by that box. There are several methods of controlling this paradigm:
- Normal Flow: `position:static` block elements each occupy their own line, appearing in a single column 
- Relative Positioning: `position: relative` normal positioning with manual adjustments to individual elements
- Absolute Positioning: `position: absolute` The position of the element is strictly defnined and ignores other elements on the page
- Fixed Positioning: `position: fixed` positioning relative to the browser window and nothing else
- Floating Elements: `float: directionca`one element floats in a position, and other content bends around it. 
`z-index` allows the developer to control which elements belong on top when they overlap

## Duckett JavaScript 3 pt. 1: Functions, Methods, and Objects
*parts of these notes spliced in from 102-7*


**Functions** are predefined operations that you can code and then call upon many times. they generally require **parameters** and then produce a **Return Value**.
A function can be declared in the form 
`function functionName() {}` 
and then called later with simply `functionName()`, making performing the function's operations many times much simpler.
If information is needed, the function can be declared as `function functionName(info1, info2) {}` and then use the collected variables in its operations. 
You can then use `return` and let the returned value be stored in a variable or array. 
Functions can also return an array if it is necessary to return multiple items. They can also be called withing one another to efficiently pass returned values from one function to the next, and can also be evoked immediately upon establishment by wrapping them in parentheses. Keep in mind that variables within functions only exist while function is running: Only the returned value can escape the underworld. 


## Allie Grampa: 6 Reasons for Pair Programming
This article can be found [here.](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

Grampa gives an overview of pair programming, a technique for collaborating on coding projects said to dramatically increase productivity and accuracy. As the title suggests, Allie has several reasons to present:

1. Increased Efficiency
Expedited problem solving and increased accuracy, along with a healthy dose of positive working conditions.
2. Engaged Collaboration
With partner, it is much easier to maintain focus and get problems solved, either through collaboration or otherwise. 
3. Learning from each other
The developers that are working together will inevitably share skills, helping them both learn and improve.
4. Social Skills
Pair programming requires and therefore developes communication skills and teamwork. 
5. Interview readiness
Pair programming is a common interview tactic, so being comfortable with it can give you an edge in this style of interview. 
6. Work Environment Readiness
Similarly, there are a plethora of companies that operate with pair programming day-to-day, and having a background in the process means you will be more prepared for those jobs. 