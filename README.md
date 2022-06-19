
Let’s learn about list comprehensions! You are given three integers **_x_**, **_y_** and **_z_** representing the dimensions of a cuboid along with an integer **_n_**. Print a list of all possible coordinates given by (_**i**_, _**j**_, _**k**_) on a 3D grid where the sum of _**i**_ + _**j**_ + _**k**_ is not equal to **_n_**. Here, **0** <= **_i_** <= **_x_; 0 <= _j_ <= _y_; 0 <= _k_ <= _z_**. Please use list comprehensions rather than multiple loops, as a learning exercise.

**Example**

**x = 1**  
**y = 1**  
**z = 2**  
**n = 3**

All permutations of [_**i**_, _**j**_, _**k**_] are:  
**[**[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 1, 0], [0, 1, 1], [0, 1, 2], [1, 0, 0], [1, 0, 1], [1, 0, 2], [1, 1, 0], [1, 1, 1], [1, 1, 2]**]**.

Print an array of the elements that do not sum to _**n**_ **_=_** **_3_**.  
**[**[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 1, 0], [0, 1, 1], [1, 0, 0], [1, 0, 1], [1, 1, 0], [1, 1, 2]**]**

## **Input Format**

Four integers **_x_**, _**y**_, _**z**_ and **_n_**, each on a separate line.

## **Constraints**

Print the list in lexicographic increasing order.

**Sample Input 0**

```
1
1
1
2
```

**Sample Output 0**

```
[[0, 0, 0], [0, 0, 1], [0, 1, 0], [1, 0, 0], [1, 1, 1]]
```

**Explanation 0**

Each variable **_x_**, _**y**_ and **_z_** will have values of **0** or **1**. All permutations of lists in the form [_**i**_, _**j**_, _**k**_] = **[**[0, 0, 0], [0, 0, 1], [0, 1, 0], [0, 1, 1], [1, 0, 0], [1, 0, 1], [1, 1, 0]**]**.

Remove all arrays that sum to **_n_ = 2** to leave only the valid permutations.

**Sample Input 1**

```
2
2
2
2
```

**Sample Output 1**

```
[[0, 0, 0], [0, 0, 1], [0, 1, 0], [0, 1, 2], [0, 2, 1], [0, 2, 2], [1, 0, 0], [1, 0, 2], [1, 1, 1], [1, 1, 2], [1, 2, 0], [1, 2, 1], [1, 2, 2], [2, 0, 1], [2, 0, 2], [2, 1, 0], [2, 1, 1], [2, 1, 2], [2, 2, 0], [2, 2, 1], [2, 2, 2]]
```
