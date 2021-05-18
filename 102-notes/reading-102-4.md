# Working in HTML: Duckett Chapters 1, 8, 17, 18

## Duckett 18: Designing a Website

### Objectives
When creating a website, the question of audience must drive each decision. Every demographic data point is in play. 

Next, the question of purpose: why do people use your site? Entertainment? Information? Shopping? These core elements of purpose can be broken down into motivations and goals. 

Based on those goals, you can assess the information your visitors will need and begin incorporating it into how you plan your website. Each item or feature you add should tie into these core goals

How often will people visit your site? What does this mean for the need for updates? 

### Structure
Once you have assessed what your site will need to do, you are able to construct a site map that outlines the pages you will need and what each section of each page will accomplish. 

Sketch out a wireframe for each page on your site that delineates where the critical items on each page will be located and how much space will be allocated to them. 

### Visual Design
Use visual hierarchy and and visual distinction to control where focus is placed in your webpage so that the most important information is always observed. Organize pages in a logical fashion to make it easier for users to parse information. 
- Size, color, and style can all be used to create visual hierarchy. 
- Visually grouping similar items can help the user understand which items are related.
- Navigation should be kept short and concise for clarity, with less common destinations kept separate from the main navigation. 

## Duckett 01: HTML Structure
HTML elements are contained within opening and closing tags '<></>' and tell a browser how to display the information. 
- tags `<html></html>` contain HTML code
- `<h1>` and `<h2>` create headers and subheaders
- `<p>` contains a paragraph
- attributes can be added within the tags to alter their elements
- `<head>` contains information about the page rather than in the page, such as...
- `<title>` gives the website a title atop the browser
- `<body>` contains everything that exists in the main browser page

## Duckett 17: HTML5 Layout
HTML5 offers specific tags for creating a clearer structure to your websites. 
- `<header>` and footer can contain common content for their respective parts of the site
- `<nav>` (navigation) contains the primary naviagation bar for the website, and sometimes a second nav will contain the secondary navigation options. 
- `<article>` contains content that can operate independently. 
- `<aside>` is used to identify supporting information, whether for an article or the overall site.
- `<section>` will usually have its own header, and groups a particular type of content. 
- `<hgroups>` allows you to group headings together to combine them (?)
- `<figure>` denotes content within an article that could be removed, usually an unnecessary reference image or quote. 
- finally, `<div clas="noun">` can be used to subdivide and content not covered by the above tags. 

Duckett 17 also covers code to help old browsers interpret HTML5, and the use of `<a></a>` to make a block of content into a link. 

## Duckett 8: Extra Markup
This chapter covers additional details needed to create a cohesive webpage:
- Each webpage should begin with `<!DOCTYPE html>` or similar to identify the type of code being presented. 
- `<!-- -->` allows for line commentary within HTML
- `id="identifier"` is a global attribute that can be used to add a unique referencable value to any tag. 
- similarly, `class="identifier"` can be used to give a similar value, but one to used multiple times on similar tags. 
- Block elements begin on their own line, such as `<h1>`, `<p>`, `<ul>`, and `<li>`. 
- Not so for inline elements like `<a>`,`<b>`,`<em>`, and `<img>`.
- `<span>` allows for some subset of content to be tagged inline with an identifier for use with CSS
- `<iframe>` or "inline frame" lets you display a window to another site on your page. They can have several attributes: 
  *  `src="url.com"` provides a source webpage
  * `height="###"` and `width="###"` set size parameters
  * `seamless` removes scrollbars on the iframe
- `<meta>` stores metadata in the head via attributes. These mostly interact with search engines and browsers and tell them how to handle a webpage. 
- Escape characters are avaliable to display characters used in HTML code, like brackets or quotation marks. 


[<<Return to Home](README.md) 