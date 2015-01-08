Pointers, references and functions
=====================

Welcome to the world of functions! This is maybe the most important material for the whole semester so you'd better feel confident in your skills related to these. In order to help you achieve that, here are some tasks. Wherever you're asked to write only a function you should write only the function, no includes no namespaces no main functions, only the wanted function!

###NB!!!!!!!!!
In case you don't know what a function prototype is check [this](http://en.wikipedia.org/wiki/Function_prototype)

##Task1: Change me!
You're to implement a function, which has the following prototype:

```void changeArr(int* arr, int start, int end, char operation, int number) ```

* arr is a pointer to an array and we aim to change some of it's elements;
* start is the index of the first element that should be changed;
* end is the index of the last element that should be changed;
* operation is one of the following '+', '-', '*';
* number is a number which should be used in changing of the elements;

So basically the function should change some of the elements of the array by adding, substracting or multiplying by a specific number.


##Task2: Pizza order
Write a C++ function which has the following prototype:

```
bool isLoyal(char client[], char loyalClients[][10], int loyalClientsCount, double& prize)
```

* client is the name of the client;
* loyalClients is an array with all the first names of loyalClients of our Pizzeria;
* loyalClientsCount is the count of the loyal clients which are passed to the function;
* prize is the prize of the order that the client wants to make;

The function should check if the client is loyal and return true if yes, otherwise false. If the client is loyal we should make a 25% discount to the prize of his order.

###That's it now get to work!
