# 201-13 Notes: Mark Pilgrim on Local Storage

This article is available [here.](http://diveinto.html5doctor.com/storage.html)

The first section of the article gives an overview of the trials and tribulations of local internet storage. Suffice it to say that many ideas were tried, and few were widely usable. 

HTML5 introduced local storage functionality for key:value pairs, which is now supported by all most modern browsers. Data is stored with a string for a key that corresponds to any form of data as a value. 

localStorage can be handled as an object with the stored data as properties, and .getItem and .setItem used as methods to access them. Bracket notation also works to manipulate these properties. 

changes made to localStorage generate events, which can be logged with eventlisteners to keep track. localStorage is limited to 5 megabytes, and there really isn't a practical way to get around that. 

Apart from localStorage, SQL and IndexedDB are scattered alternatives to solving the same issues. There is also a plethora of further reading to be called upon on the subject at the end of this article. 


[<<Return to Home](README.md)