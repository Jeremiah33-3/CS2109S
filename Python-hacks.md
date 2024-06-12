## List Comprehension

> A Python list comprehension consists of brackets containing the expression, which is executed for each element along with the for loop to iterate over each element in the Python list.

General syntax:
`new_arr = [num for num in arr]`

With arithmetic operations:
`new_arr = [num ** 2 for num in arr]`

With logical operations:
`new_arr = [num for num in arr if num % 2 == 0]`

Matrix:
`matrix = [[j for j in range(3)] for i in range(3)] `

## Indexing and slicing

Negative indexing, e.g. `arr[-n]` means accessing the nth last element in the list 
- `arr[-1]` means accessing the last element of the list

Slicing: `a[m:n]` means return a portion of the list starting with postion m, up to but not including n.
Can works for negative index: a[-m:-n] where m > n means accesing the mth last element up to but not including the nth last element. 

Omitting values in slicing:
Omitting the first index a[:n] starts the slice at the beginning of the list.
Omitting the last index a[m:] extends the slice from the first index m to the end of the list.
Omitting both indexes a[:] returns a copy of the entire list, but unlike with a string, it’s a copy, not a reference to the same object. // side note: can check using `==` operator as well as `is` operator; The `==` operator is used to compare the equality of objects. The `is` operator is used to check if different variables are pointing to the same object in memory

Stride/step can be added (the third index) to determines the interval in which the elements are taken at.
