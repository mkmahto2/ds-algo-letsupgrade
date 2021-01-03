# Assignment number 2
#### Question 1
## Write the program for deleting an element from the beginning and from any position.

~~~


#include <stdio.h>
int main()
{
   int array[100], position, c, n;

   printf("Enter number of elements in array\n");
   scanf("%d", &n);

   printf("Enter %d elements\n", n);

   for (c = 0; c < n; c++)
      scanf("%d", &array[c]);

   printf("Enter the location where you wish to delete element\n");
   scanf("%d", &position);

   if (position >= n+1)
      printf("Deletion not possible.\n");
   else
   {
      for (c = position - 1; c < n - 1; c++)
         array[c] = array[c+1];

      printf("Resultant array:\n");

      for (c = 0; c < n - 1; c++)
         printf("%d\n", array[c]);
   }

   return 0;
}
~~~
#### Question 2

Q.Write the program for printing the array after rotating it k times towards left, where k
would be taken as user input.

~~~
// C++ program to rotate an array by 
// d elements 
#include <bits/stdc++.h> 

using namespace std; 

  
/*Function to left Rotate arr[] of  

  size n by 1*/

void leftRotatebyOne(int arr[], int n) 
{ 

    int temp = arr[0], i; 

    for (i = 0; i < n - 1; i++) 

        arr[i] = arr[i + 1]; 

  

    arr[i] = temp; 
} 

  
/*Function to left rotate arr[] of size n by d*/

void leftRotate(int arr[], int d, int n) 
{ 

    for (int i = 0; i < d; i++) 

        leftRotatebyOne(arr, n); 
} 

  
/* utility function to print an array */

void printArray(int arr[], int n) 
{ 

    for (int i = 0; i < n; i++) 

        cout << arr[i] << " "; 
} 

  
/* Driver program to test above functions */

int main() 
{ 

    int arr[] = { 1, 2, 3, 4, 5, 6, 7 }; 

    int n = sizeof(arr) / sizeof(arr[0]); 

  

    // Function calling 

    leftRotate(arr, 2, n); 

    printArray(arr, n); 

  

    return 0; 
} 
~~~
