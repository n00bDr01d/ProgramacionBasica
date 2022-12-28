# Problem: Christmas Tree

Write a program that takes a number **n** (1 ≤ n ≤ 100) and prints a Christmas tree with height of **n+1**.

| Input | Output                                          | Input | Output                                                                      |
| ----- | ----------------------------------------------- | ----- | --------------------------------------------------------------------------- |
| 1     | <p>  <code>|</code>  <br><code>* | *</code></p> | 2     | <p>   <code>|</code>   <br> <code>* | *</code> <br><code>** | **</code></p> |

| Input | Output                                                                                                      | Input | Output                                                                                                                                          |
| ----- | ----------------------------------------------------------------------------------------------------------- | ----- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| 3     | <p>    <code>|</code>    <br>  <code>* | *</code>  <br> <code>** | **</code> <br><code>*** | ***</code></p> | 4     | <p>     <code>|</code>     <br>   <code>* | *</code>   <br>  <code>** | **</code>  <br> <code>*** | ***</code> <br><code>**** | ****</code></p> |

## Video: Christmas Tree

Watch this video lesson to learn how to print a Christmas tree on the console using nested loops: https://youtu.be/UecoBfhUIkk.

## Hints and Guidelines

From the examples we see that **the Christmas tree** can be **divided** into **three** logical parts. **The first** part is **the stars and the white spaces before and after them**, **the middle** part is **`|`**, and **the last** part is again **stars**, but this time there are **white spaces** only **before** them. The printing can be done with only **one loop** and the **`new string(…)`** constructor, which we will use once for the stars and once for the white spaces.

![](../../../assets/chapter-6-images/07.Christmas-tree-01.png)

## Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/512#6](https://judge.softuni.org/Contests/Practice/Index/512#6).
