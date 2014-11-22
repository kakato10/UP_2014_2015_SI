Nested loops, multidimensional arrays and "strings"
=====================

Okay, dokey. Let's see how nested loops look like.
```
int array[10];
for (int i = 0; i < 9; i++) //gonna call it loopOne
{
	for (int j = i + 1; j < 10; j++ ) //gonna call it loopTwo
	{
		//do some code here using array[10]
	}
}
``` 
In that case we have a loop that will iterate through the array (loopOne).
Why the condition in the for loop is ``` i < 9 ``` ? Take a look at loopTwo. Notice that
``` j = i + 1 ``` in that case if ```i = 9``` then j will be 10 and we dont't have an element with index 10 in the array so will get an error. 
Now what is actually happening with that nested loops?
For every iteration of loopOne, loopTwo will go ahead of it and check all the values in the array. If the array is big the process is very slow so be careful when using nested loops in production.
In that [link](http://mathbits.com/MathBits/CompSci/looping/nested.htm) you can find a bit more concrete explaination how does this works. This explaination refers to every other loops too.
Notice that we can make while loop inside for loop and every possible combination between loops.

Now this is a multidimensional array:
```
int t[4][2] = [[1, 3], [0, 2], [12, -2], [1, 9]];
```
We can use the for representing matrixes that we use in maths.
This was a two dimensional array. Of course you can have four, five and so on dimensional arrays but they are not used very often.
[Here](http://www.learncpp.com/cpp-tutorial/65-multidimensional-arrays/) you can learn a bit more about them.

Well about Charecter arrays (also called "strings") check the following links:
* https://www.youtube.com/watch?v=S7K9y-A0fxc
* http://www.cplusplus.com/doc/tutorial/ntcs/
