Nested loops, multidimensional arrays and "strings"
=====================

Well it's time to take a look at something a bit more complicated. You already know what is a loop and an array. This time we'll take a look of nested loops and multidimensional arrays, for what are we using them and what'sthe connection between them. You can find that info in materials.md

Now let's take a look at the tasks for today.

##Task1: Basic matrix operations
You're to implement a C++ program which asks the user to enter the elements of 4x4 matrix.
There's no need to validate the input. After that you should ask the user to enter an operation that he wants to be done by the program. The possibilities are the following:
* sum two matrixes (the second matrix is again 4x4). User input is '+';
* substract two matrixes (the second is again 4x4). User input is '-';
* multiply the elements of the matrix with a number entered by the user. User input is '*';
* devide the elements of the matrix with a number entered by the user. User inpput is '/';

For sum and substract use the following matrix as second:
```
 1  0  4  10
11  5  7   1
 0  0  2   1
 3  2  8   0
```
Use switch statement for that task.

###Example1
Input:
```
Matrix:  3  2  1  5
		 7  1  0 12
		 0  1 -2  1
		 3  9  4 -2
Operation: '+'

```
Output:
```
Result:  4  2  5  15
		18  6  7  13
		 0  1  0   2
		 6 11 12  -2
```

###Example2
Input:
```
Matrix:  3  2  1  5
		 7  1  0 12
		 0  1 -2  1
		 3  9  4 -2
Operation: '*'
Number: -1

```
Output:
```
Result:  -3  -2  -1  -5
		 -7  -1   0 -12
		  0  -1   2  -1
		 -3  -9  -4   2
```

##Task2: lexicographic comparison
Write a C++ program which asks the user to enter two strings with length no more than 6 characters. After they're entered the program should compare them and tell the user which string is "bigger".
Let's asume that str1 is the first string and str2 is the second one. The rules that your custom comparison should follow are:.
* if the code of str1[i] is bigger than str2[i] then str1 is bigger than str2;
* if str2 has ended before str1 and they were equivalent until that moment str1 is bigger;
* if str1 and str2 are ending and the same time and the were equivalent until now they are equivalent.

###Example1
Input:
```
str1 = "Cool"
str2 = "cool"
```
Output:
```
str1 < str2
```
###Example2
Input:
```
str1 = "cool"
str2 = "cool"
```
Output:
```
str1 = str2
```
###Example3
Input:
```
str1 = "cooling"
str2 = "cool"
```
Output:
```
str1 > str2
``` 

###Ready! Steady! GO!!!!!!

