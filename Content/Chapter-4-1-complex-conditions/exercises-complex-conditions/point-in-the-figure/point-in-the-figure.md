# Problem: \* Point in the Figure

The figure consists of **6 blocks with size h \* h**, placed as in the figure below. The lower left angle of the building is on position {0, 0}. The upper right angle of the figure is on position {**2\*h**, **4\*h**}. The coordinates given in the figure are for **h = 2**:

![](../../../../assets/chapter-4-images/13.Point-in-the-figure-01.png)

Write a program that enters an integer **h** and the coordinates of a given **point {x, y}** (integers) and prints whether the point is inside the figure (**inside**), outside of the figure (**outside**) or on any of the borders of the figure (**border**).

## Sample Input and Output

| Input               | Output  | Input              | Output |
| ------------------- | ------- | ------------------ | ------ |
| <p>2<br>3<br>10</p> | outside | <p>2<br>3<br>1</p> | inside |

| Input              | Output | Input              | Output |
| ------------------ | ------ | ------------------ | ------ |
| <p>2<br>2<br>2</p> | border | <p>2<br>6<br>0</p> | border |

| Input              | Output  | Input                 | Output  |
| ------------------ | ------- | --------------------- | ------- |
| <p>2<br>0<br>6</p> | outside | <p>15<br>13<br>55</p> | outside |

| Input                 | Output | Input                 | Output  |
| --------------------- | ------ | --------------------- | ------- |
| <p>15<br>29<br>37</p> | inside | <p>15<br>37<br>18</p> | outside |

| Input                | Output  | Input                | Output |
| -------------------- | ------- | -------------------- | ------ |
| <p>15<br>-4<br>7</p> | outside | <p>15<br>30<br>0</p> | border |

## Hints and Guidelines

A possible logic for solving the task (not the only correct one):

* We might split the figure into **two rectangles** with a common side:

![](../../../../assets/chapter-4-images/13.Point-in-the-figure-03.png)

* A point is **outer (outside)** for the figure, when it is **outside** both of the rectangles.
* A point is **inner (inside)** for the figure, if it is inside one of the rectangles (excluding their borders) or lies on their common side.
* In **other case** the point lies on the border of the rectangle (**border**).

## Implementation of the Proposed Idea

An exemplary implementation of the described idea (parts of the code are blurred with the purpose of stimulating logical thinking and solving skills):

![](../../../../assets/chapter-4-images/13.Point-in-the-figure-02.png)

## Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/508#12](https://judge.softuni.org/Contests/Practice/Index/508#12).
