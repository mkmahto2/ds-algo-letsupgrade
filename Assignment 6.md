### Question 1
#### Write a function to find the maximum element in the stack.
// C++ program to implement a stack that supports 
// getMaximum() in O(1) time and O(1) extra space. 
#
~~~
## Question 2
Write a function to find the minimum element in the stack.
~~~

// CPP program to find 
// minimum (or maximum) element
// in an array.
#include <bits/stdc++.h>

using namespace std;
 

int getMin(int arr[], int n)
{

    // If there is single element, return it.

    // Else return minimum of first element and

    // minimum of remaining array.

    return (n == 1) ? arr[0] : min(arr[0], 

                         getMin(arr + 1, n - 1));
}
 

int getMax(int arr[], int n)
{

    // If there is single element, return it.

    // Else return maximum of first element and

    // maximum of remaining array.

    return (n == 1) ? arr[0] : max(arr[0], 

                          getMax(arr + 1, n - 1));
}
 

int main()
{

    int arr[] = { 12, 1234, 45, 67, 1 };

    int n = sizeof(arr) / sizeof(arr[0]);

    cout << "Minimum element of array: " << 

                            getMin(arr, n) << "\n";

    cout << "Maximum element of array: " << 

                                   getMax(arr, n);

    return 0;
}
~~~
