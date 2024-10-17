# Functions

## Aim
To demonstrate the use of pointers in C++ by swapping the values of two variables using a function.

## Theory
Pointers are variables that store the memory address of another variable. By using pointers, we can directly manipulate the values stored in memory. This is particularly useful for functions that need to modify the actual values of arguments passed to them.

## Algorithm
1. Define a function `swap` that takes two integer pointers as parameters.
2. Inside the function, declare a temporary integer variable `temp`.
3. Assign the value pointed to by the first pointer to `temp`.
4. Assign the value pointed to by the second pointer to the location pointed to by the first pointer.
5. Assign the value stored in `temp` to the location pointed to by the second pointer.
6. In the `main` function, declare two integer variables `a` and `b` and initialize them.
7. Call the `swap` function, passing the addresses of `a` and `b`.
8. Print the swapped values of `a` and `b`.

```cpp
#include <iostream>
using namespace std;

void swap(int *x, int *y) {
    int temp;
    temp = *x;
    *x = *y;
    *y = temp;
}

int main() {
    int a = 5, b = 2;
    swap(&a, &b);
    cout << "value of a: " << a << endl;
    cout << "value of b: " << b << endl;
    return 0;
}
