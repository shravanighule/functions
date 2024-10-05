Functions
Aim
To study pointer operations

Software Used
Visual studio code

Theory

In C++, functions can receive parameters in different ways, influencing how the function manipulates the provided values. Two common methods are Call by Reference and Call by Value:
Call by Reference
Definition: Call by Reference means passing the address (reference) of the actual parameters to the function. This allows the function to modify the original values.

Working: The function receives pointers to the variables, and operations performed inside the function affect the original variables directly.

Call by Value
Definition: Call by Value means passing a copy of the actual parameters to the function. Changes made to the parameters inside the function do not affect the original variable

Algorithms
Call by value
1.Start
2.Define Function swap(int x, int y)
Input: Two integers x and y
Output: Swapped values of x and y
Inside Swap function:
Create a temporary variable temp
Assign the value of x to temp
Assign the value of y to x
Assign the value of temp to y
3.Inside main Function
Define two integers a and b with 5 and 2
Call swap(a, b)
Print the value of a
Print the value of b
4.End
