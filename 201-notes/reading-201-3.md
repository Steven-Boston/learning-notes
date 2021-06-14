# Lists, Control Flow, and the Box Model 
## Duckett HTML/CSS 3: Lists
This quick chapter loads the reader up on different list tags:
- `<ol>` with `<li>` within creates an ordered list, numbered by default.  
- `<ul>` with an `<li>` within reduces that default to bullet points
- `<dl>` is used for a list of definitions (`<dd>`) of terms (`<dt>`)
Duckett also points out that a list item may in fact feature another list, and if so the browser will add another level of indentation with a secondary bullet point style. 

## Duckett HTML/CSS 13: Boxes
SUNDAY SUNDAY SUNDAY! CSS HAS A BONE TO PICK WITH THAT INDEX.HTML FILE, AND BOXING IS ITS PRIMARY MEANS OF INTERACTION. BY THE TIME CSS IS DONE WITH IT, THAT WEBPAGE IS GONNA HAVE HAD ITS BOXES SET TO NEW DIMENSIONS WITH `height: 200px; width: 70%` AND SIMILAR EFFICIENT TACTICS FOR REWRITING BOX DIMENSIONS. CSS IS THROWING DOWN NEW LIMITS ON THOSE BOXES WITH `min-width: 20px` AND `max-height: 650px;`. AND IF THAT HTML THINKS THE CONTENT CAN JUST OVERFLOW FROM THE NEWLY LIMITED BOX, CSS IS GONNA USE `overflow: hidden;`  or `overflow: scroll;` TO SEND THAT EXTRA CONTENT PACKING. HTML BETTER NOT BE COUNTING ON THAT DEFAULT PADDING (or margin or border) BECAUSE CSS MIGHT JUST TAKE IT ALL AWAY OR PUT SOME MORE ON WITH
`border: style widthpx color`
or `margin: toppx rightpx bottompx leftpx;` 
or even `padding: toppx rightpx bottompx leftpx;`

BUT THAT'S NOT ALL FOLKS, CSS IS GONNA BE SENDING HTML'S BOXES FROM ONE END OF THE PAGE TO THE OTHER WITH `text-align: direction;` ONCE THOSE BOXES HAVE HAD THEIR DIMENSIONS SET. WITH THAT DOCTYPE TAG, EVEN IE6 WON'T BE ABLE TO SAVE HTML FROM WHAT CSS IS COOKING. HTML AND THE BROWSER THOUGHT THOSE BOXES WERE ARE GOING TO HAVE THEIR OWN BLOCK, BUT CSS IS BRINGING THE PAIN WITH `display: inline;`, ONLY TO BRING THEM RIGHT BACK TO THE BLOCK WITH `display: block`, AND WITH `display: inline-block` READY AND WAITING, HTML'S BOXES ARE AT CSS'S MERCY. TICKETS ARE ON SALE NOW, AND THOUGH EACH ONE PAYS FOR THE WHOLE SEAT, THE ONLY PART OF THIS BOX MODEL YOU'LL NEED IS *THE BORDER*

Anyway, there are a couple more tricks to spruce up a box on the webpage:
- `border-image: url('pic.com')  sliceAtpx sliceAtpx sliceAtpx sliceAtpx stretch;` turns the linked image into a custom border (the last value can also be repeat or round, according to how the image is to be handled) -moz- and -webkit- before the beginning of the key will help older browsers display the image border. 
- `box-shadow: hoffsetpx voffsetpx blurdistancepx spreadpx color` adds a drop shadow to the box, as defined by the color and positional values. Add inset to the list of values to invert the shadow to the box's interior. 
- `border-radius: cornerRadiuspx` forms an established border into rounded corners around the specified radius. 4 values can be provided to control the corners individually (TRBL), or individual lines (`border-top-right-radius:`) to the same effect
- by using a line for an individual corner or by specifying four horizontal and then four vertical values, the corners can be manipulated to curve in uneven bends. 

## Duckett JS/JQ 2: 
*This review of pp. 70-73 from yesterday covered Arrays. Yesterday I wrote:*
### Arrays
Arrays are a type of variable that can store multiple values (generally a list). they can be created using brackets [] when manipulating the variable and separating each value with a comma in the form

`var thingsList = ['thing1', 'thing2', thing3']`

alternatively, `new Array();` can be used. Once the array is established,  you can reference a particular array item via `thingslist[0]`. Keep in mind that arrays begin at position 0. 


## Duckett JS/JQ 4 pt. 2: Loops & Switches
### Switch Statements
switch statements come in the form `switch (indicator) {}`, with several cases defined with different code to execute.
```
    switch (indicator) {
      case: 'yellow': 
        fruit = 'banana';
        break;
      case: 'red':
        fruit = 'apple';
        break;
    }
```
This can be useful in a situation with many possible outcomes demanding different action. 
### Actual reality vs. Java reality
Some things are the same, and some are the same only in the eyes of Javascript. Javascript will attempt to convert values of an unexpected data type to avoid errors, but just like a child trying to avoid getting caught after breaking something, hiding the problem can be even more trouble. Bring your comparisons back into the real world by using === instead of == (or !== instead of !=). With this, you can make JavaScript realize that a string of 'one' is in fact not a number. without it, well...
![Primrose!](./primrose1.jpg)
....at least it will having liking strings too much in common with Primrose. 

Oh, and while we are here, this rather cavalier attachement to the truth that JavaScript has bleeds over to, well, the truth. With Javascript, some things true-ish or false-ish. Or **Truthy** or **Falsey** if you like:

Falsy Things:
- `0` The number. Just Zero. 
- `''` Things that aren't there in a blank string. 
- `3/'bears'` things that might be Kingdom Hearts titles but certainly are not numbers. At least I am on board with this one. 
- `noValue` a variable with nothing in it is falsy.

In the Truthy Corner:
- `653` All the other numbers. What did zero do to you Javascript?
- `'the earth is flat'` strings with words. doesn't matter what they are. 
- `2.3/6.8` come on... this has to be worse than zero. 

If statements can use this lasse-faire method of verification to make `if (variable){}` be a check for the existence of the variable before proceeding. Note that `if (variable == true) {}` still won't get it done. Even JavaScript has limits on what passes for truth. 

Logical operators have an odd application: They actually give the value of the item that caused them to cease their operations, meaning that `item1 = ( item2 || item3 )` will make item1 into whichever of item2 or item3 happens to exist first, starting from the left. 

### Loop (There it is)

*starting with some notes from 102.8*
**Loops** check a condition and continually execute a set of actions some number of times. **for()** loops, which are generally used to execute an action a specific number of times, using a counter as a condition and increment that counter each execution. For example:
`for(var n = 0; n<20; n++) {}`
will create a loop that checks n is less than 20, and executes the code if that is true, increments the value of n, and repeats, presumably twenty times. 
**while** and **do while** loops are useful when the number of repetitions is unknown or depends on the input. 
    var n = 0 
    var names = ''
    while (n<6) {
    names += ' ' + prompt('what is your name?')
    n++;
    } ```
The above creates a loop similar to a for loop, but similar tactics could be used with slightly altered code to increment only if a response were given, and continue until 6 responses had been collected. 

174-5 add some *loopy* vernacular:
- break will let you escape the simulation (meaning the loop)
- continue puts you back at the top of the loop so that you can check the conditions right away. 
These useful pages also make mention of looping in order to run through each item of an array and use the same code on it, and then breaks down how to do it, including the useful `arrayLength = arrayName.length;` in order to determine the length of the array before rolling through it by calling `arrayName(i)` in the loop actions, where i is the loop counter. 
 



[<<Return to Home](../README.md)