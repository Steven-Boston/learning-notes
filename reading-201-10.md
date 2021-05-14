# Duckett JS/Jquery 10: Debugging

This chapter outlines the process of debugging code, or more specifically, the process of ascertaining the source of buggy code. When searching for the source of an error, it is important to follow the lineof execution and consider the context in which the problem is likely to be occurring. Does the problem stem from a function? Or an event handler? What prior steps do the relevant code blocks rely on? All of these factors can help sleuth out the source of errant results. 

Javascript works though the code one line at a time, and when it detects that a line requires another to function, it stacks the needed line on top of the first like a counterspell, and then the stack resolves just as it would otherwise. 

When Javascript finds an error, it checks for a way to resolve the error, and if none applies, it throws an exception and stops processing the code. Errors come in many shapes and sizes:
- SyntaxError: you need a closing bracket. Maybe a semicolon. 
- ReferenceError: The referenced variable does not exist
- TypeError: Data is the wrong type. 
- RangeError: A number is not in a manageable range. 
Duckett describes two options we are faced with when errors occur: 

1. Debug the errors
2. Handle them gracefully

The process of debugging outlined in this chapter is primarily a tutorial on wielding the dev tools and the console. As I am already comfortable with those processes, I instead focused on handling errors with grace:

`try{}`, `catch(exception){}`, and `finally{}` form the special task force for handling exceptions. Try is in the business of keeping an eye on the suspicious code that might fail. When it does fail, catch will step in and run its code to cover the error or display a message to the user. Finally is there to make a dramatic exhale and (ideally) put us back on track. Or at least on some sort of track. 

In cases where we can see an error coming down the line, it can be useful to take matters into our own hands. `throw new Error('explanation')` manually forms an error and informs the user, saving time and energy waiting for it to inevitably arrive later. 

[<<Return to Home](README.md)