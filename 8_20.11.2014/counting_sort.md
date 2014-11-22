Counting sort
=====================
During the exercise we took a "glance" at the counting sort.
In that[link](https://www.youtube.com/watch?v=o3FUC6l89tM) you can find a video explaining the algorithm one more time.
Here is a basic C++ implementation of the algorithm. REMEMBER IT ONLY WORKS FOR POSITIVE INTEGERS!

```
#include <iostream>
using namespace std;

int main()
{
	int pause;
	int arr[] = { 2, 5, 1, 5, 7 };
	
	//the length of result_indexes should be the biggest element in arr (this case 7) plus 1
	int result_indexes[8] = { 0, 0, 0, 0, 0, 0, 0, 0 };
	
	//the length of result should be the length of arr plus 1
	int result[6];

	//with this for loop we are telling the result_indexes which elements do we have in the array that we want to sort
	for (int i = 0; i < 5; i++)
	{
		result_indexes[arr[i]] += 1;
	}
	//after the loop has finished it's filled with {0,1,1,0,0,2,0,1}

	//with this for loop we're going to find which are the indexes on which we should place the elements from arr into result
	for (int i = 1; i < 8; i++)
	{
		result_indexes[i] = result_indexes[i] + result_indexes[i - 1];
	}
	//after the loop has finished it's filled with {0,1,2,2,2,4,4,5}

	//in this for we're going to fill the result array
	//for every element of the arr, that we want to sort, we're going to ask the second 
	//array on which index should it be put in the result arr
	for (int i = 0; i < 5; i++)
	{
		result[result_indexes[arr[i]]] = arr[i];
		
		//with the line below we're going to take care for every element that is met twice or more in the first arr
		//to be put on the respective indexes
		//for example in arr we have two times 5. The index that the result_indexes will give us the first time we ask for 5 will
		//be 4 but 5 should be on index 3 too so we substract 1 from 4 and we get that the second 5 should be placed on index 3
		result_indexes[arr[i]] -= 1;
	}

	//notice that we didn't do anything with result[0] so in that element there can be any kind of value
	//and we don't want to show it to the user
	for (int i = 1; i <= 5; i++)
	{
		cout << result[i] << endl;
	}

	cin >> pause;
	return 0;
}
```

If someone wants to learn more about sorting algorithms, take a loook at that [wikipedia page](http://en.wikipedia.org/wiki/Sorting_algorithm).