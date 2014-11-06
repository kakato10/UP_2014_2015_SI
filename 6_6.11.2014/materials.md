Enum and arrays
=====================
It's time to talk about enum and arrays. 

##Enum
We're using enum type to make our own variable types.
For example we can make a variable type named color like this:
```
enum Color {BLUE=1, RED=2, GREEN, WHITE}
```
And we can define a variable of type color like this:
```
Color my_color = GREEN
Color my_color = 4 //that means my_color is white
```
BLUE, RED and all other colors are called constants of the type Color. Every constant is presented in the memore with it's code (1 for BLUE, 2 for RED and so on).
If you don't specify the code of a constant it will get the code of the previous constant and will add 1 to it (the code of GREEN is equal to the code of RED + 1)
So basically if you do the following 
```
enum Color {BLUE=3, RED=4, WHITE=2, GREEN, BLACK}
```
you will have two constants with code 3 (BLUE and GREEN) and two with code 4(RED and BLACk).
So be careful when using them!
You can read more about enum over here:
* http://www.cprogramming.com/tutorial/enum.html

##Arrays

Now, let's say something. We use them to store many values of the same type in one particular variable. For example if we want to store 3 real numbers in one variable for example test_results we do one of the following;
```
double test_results [3] = {5.65, 3.20, 4.50};
double test_results [] = {5.65, 3.20, 4.50}
```
When we don't specify how many elements of the array are there going to be (a.k.a [] in the declaration is empty) we can add as many elements as we want in it.
Every element of the array has it's own index. The index of the first element in an array 0, the index of the second is 1 and so on until we reach the index of the last one which is the length of the array minus 1.

We can't do things like these:
```
int a[5], b[7];
cin >> a >> b;
```
```
int a[5], b[7];
a=b;
```

We can access directly an element of an array using it's index. Let's assume that we have an array of real numbers called test_results with 5 elements. We can display the third elements of the array with this: ``` cout << test_results[2] << end; ```  

You can take a look at the link below for some additional info (it will be useful):
* http://www.cplusplus.com/doc/tutorial/arrays/

