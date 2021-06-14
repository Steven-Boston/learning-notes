# Duckett Javascript: Comparisons and Loops

## Comparisons and Logical Operators (150-151, 156, 157) 
==, !=, >, <, >=, and <= (and === and !==) allow for **comparisons**, which return a true or false value by comparing two objects. 

**logical operators** allow for the comparison of multiple comparison  operators in tandem. && checks if all items meet a condition, `||` checks if at least one item meets a condition. ! will invert an otherwise normal comparison, giving the opposite boolean. Logical operators evaluate left to right, and stop when the collected results are sufficient to make a determination. 

## For and While Loops (170-173, 176)
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


[<<Return to Home](../README.md)