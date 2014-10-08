Materials and tasks for the second Introduction to Programming exercise
=====================

So we've learned something about C++ so now it's time for practice.

### Task 1 Variable changer
Task: Write a program which asks the user to enter two variables and when entered it changes their value.

Example:
	Input: 
'''
	a = 2, b = 3
'''
	Output: 
'''
	"The current value of a is 3"
	"The current value pf b is 2"
'''


### Task 2 Terminal master

Write a shell(terminal or cmd script) which:
* displays the "Hello world" message
* creates new folder named "create_me"
* deletes the "create_me" folder
* renames the "create_me" folder to "delete_me"
* deletes the "delete_me" folder
* displays the username which is currently logged in on the computer
* displays the ping of your internet connection (for Windows users)
* displays the stats of your internet connection (for linux users)
* exits the shell

This one is a little bit more hardcore. You're going to need some additional materials.
 * Windows users should check this link: http://ss64.com/nt/
 * Linux users will have to look here: http://ss64.com/bash/

In order to make make the script you will need text editor to write the commands in a file.
And what about saving it?
 * Windows users should save it with .cmd extension
 * Linux users don't need to add a specific extension. But when the file is saved they have to open the terminal, get to the folder where the file is being stored and do as follows (assuming that the file is name "script"):

 ```
 	chmod 700 script
 ```
This will make the script an executable file and now we can start it like this:

```
	./script
```

Ahhh I alomst forgot. Linux users please write this line as first in your script. ALWAYS!!!!!

```
	#!/bin/bash
```


That's it! Now get to work!