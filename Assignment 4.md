## Question 1
In the Binary Search algorithm, it is suggested to calculate the mid as
beg + (end - beg) / 2 instead of (beg + end) / 2. Why is it so?

~~~
// program for calculating mid of array 
#include <stdio.h> 
#include <limits.h> 

int main() 
{ 

    int start = INT_MAX, end = INT_MAX; 

    printf("start = %dn", start); 

    printf("end = %dn", end); 

  

    // method 1 

    int mid1 = (start + end) / 2; 

    printf("mid using (start + end)/2 = %dn", mid1); 

  

    // method 2 

    int mid2 = start + (end - start) / 2; 

    printf("mid using start + (end - start)/2 = %dn", mid2); 

    return 0; 
} 
~~~

## Question 2
Write the algorithm/function for Ternary Search.
// C++ program to illustrate
// iterative approach to ternary search
 
#include <iostream>

using namespace std;
 
// Function to perform Ternary Search

int ternarySearch(int l, int r, int key, int ar[])
 
{

    while (r >= l) {
 

        // Find the mid1 and mid2

        int mid1 = l + (r - l) / 3;

        int mid2 = r - (r - l) / 3;
 

        // Check if key is present at any mid

        if (ar[mid1] == key) {

            return mid1;

        }

        if (ar[mid2] == key) {

            return mid2;

        }
 

        // Since key is not present at mid,

        // check in which region it is present

     
