# Reading 201-9: Forms and Events

## Duckett HTML/CSS 7: Forms

Forms are used to collect user data for a variety of purposes. The basic form of... a form is:
```html
<form action="somewhere.php" method="get">
<p>Question: <input type='text' name='question' size='x characters' maxlength='x characters'/></p>
</form>
```
The form requires an **action** and a **method**. The action is the url of the destination file, and the method (get or post) determines how the text will be applied. Get adds the information onto the end of the file, post sends the data as an http header. An id attribute can also be assigned to a form for style and script referencing.

The p tag (and input tag) in the above example create a text input field. Size controls onscreen field width, but is better handled by CSS. Name establishes an identifier for the particular field. maxlength limits the number of characters the user can provide. `type='password'` creates a field that hides the entered text. 

```html
<form action="somewhere.php">
<p>Question to be posed?</p>
<textarea name='answers' cols='widthInChars' rows='#ofRows'>This will appear in the field.</textarea>
</form>
```
The **textarea** element can instead create a larger field for longer text entries with multiple lines. 

If selecting from predetermined options, **radio buttons** or **checkboxes** can be used. Both form a multiple choice question, with radio buttons allowing for 1 selection and checkboxes allowing binary responses to each of the questions. `type='radio'` or `type='checkbox'` set the input type, and separate input tags should be used for each option, and given a common name attribute to identify the question asked, as well as a value attribute that tells the server which answer was selected. Examples of these are available on pages 155-56. 

Other form options include:
- `<select>` creates a drop down list of <option>s, which can be turned into multiple select with size and multiple attributes. 
- `type=file` creates a field with a browse button following it for file submission using the post method. 
- `type=submit` adds a button to confirm a submission and send it to the server. 
- `type='image'` followed with a source attribute allows for an image to be used for a button. 
- `<button>` is an element specific to buttons, and allows text and images to be combined and synthesized into a button. 
- `type='hidden'` lets the developer create a hidden form. 
- `<label>` adds a label for the form to the file. This element can contain the form or reference it via `for='formName'`
- `<fieldset>` creates a section for multiple related forms, which can be given a title with <legend>
- `required='required'` makes a field a requirement for submission. 
- `type='date'` specifies that a date is being gathered, which standardizes some of the collection. the same can be said for `type='email'` and `type='url'`.
- `placeholder=''` adds text to a text input field until the user clicks on it. 

## Duckett HTML/CSS 14: Lists, Tables, and Forms

Predictably, CSS has several special properties to be apllied to lists, tables, and forms. `list-style-type` controls the ordering of an ordered list, or `list-style-image` can provide an image to cover bullet points. `list-style-position` with outside of inside controls where the list marker will appear related to the list item. All of these can be combined together into `list-style` for efficiency. 

pages 337-340 offer a detailed breakdown of how css properties are commonly used in lists, and introduces the useful `border-spacing`, `border-collapse`, and `empty-cells` options for controlling the details of table borders.

The remainder of the chapter covers styling techniques for forms, and introduces `:focus` and `:hover` as pseudo classes, as well as the `cursor:` property for controlling cursor display. 

## Duckett JS/Jquery 6: Events

The browser registers various forms of interaction with the user as events. These can be used to make JavaScript activate funtionality in your webpage, making it interactive. 

246 contains a large list of event types that breakdown into several categories: 
- UI events: The userinteracts with the browser.
- Keyboard events: The user manipulates the keyboard.
- Mouse events: The user wields the mouse to some effect.
- Focus events: When an element becomes (or ceases to be) the focus.
- Form events: When a form is utilized.
- Mutation events: When the DOM has been altered.
- additional HTML5 events are covered on 286-87

Next Duckett overviews the process of **event handling**:
1. Select which element or node will be responded to 
2. Choose an event that will trigger the response
3. Define the code that forms the response. 

Options for connecting (**Binding**) an element to the desired event:
- HTML Event handlers: indicate an event directly in an element's HTML attributes (don't do this).
- DOM event handlers: `targetElem.eventCode = functionToExecute`. These are limited to one function. Note that no parentheses should be used, as this would simply call the function. 
- DOM event listeners: `targetElem.addEventListener('event', functionName, boolean)` creates a moe structured approach to binding. 
- `targetElem.addEventListener('event', function() {functionName(parameter)}, boolean)` can be used if a parameter should be passed to the function. 
- Older IE versions do not support event listeners, so a simple if (targetElem.addEventListener){} else {} can be used to defines which event binding to use can be applied if necessary. 
- Default event flow for most browsers means that **bubbling** is in place (more specific elements have their events triggered first). The boolean at the end of the eventListener can be set to true to reverse this for the particular eventListener. 

Events, when registered by the browser, are passed to the functions that handle the events as an object. This event object will contain data realated to the event as properties, which can be used to drive the code in the function. The triggered function must therefore be expecting to recieve at least the event object, traditionally as e. Then, it can make use of the information provided to carry out what is needed. 

Event delegation is achieved by placing the eventListener onto a parent element with a target attribute that indicates which of the child attributes has triggered the event. This limits the number of different listeners needed and helps maintain efficiency. 

The rest of chapter 6 covers handling specific categories of events in detail. 

[<<Return to Home](../README.md)