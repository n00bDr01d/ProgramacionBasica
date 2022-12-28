# Problem: Changing Tiles

Harry has some **savings** that he wants to use to **change the tiles on the bathroom floor**. The **floor is rectangular**, and the **tiles are triangular**. Write a **program** that **calculates if his savings will be sufficient**. **Read from the console the width and length of the floor**, as well as **one of the sides of the triangle with its height towards it**. We must **calculate how many tiles are needed,** in order to cover the floor. The **number** of tiles **must be rounded up to the higher integer** and **5 more tiles must be added** as spare tiles. Also **read from the console** – **the price per tile** and **the amount paid for the work** of a workman. All prices and money calculations are performed in **`lv`** (Bulgarian levs, BGN).

## Input Data

The following 7 lines must be read from the console:

* **Savings**.
* **Floor width**.
* **Floor length**.
* **Side of the rectangle**.
* **Height of the rectangle**.
* **Price of a tile** in **lv** (Bulgarian levs, BGN).
* **Fee to be paid to the workman**.

**All** numbers must be real numbers within the range \[**0.00 … 5000.00**].

## Output Data

The following must be printed on the console as a **single line**:

* If the money **is sufficient**:
  * “{Remaining funds} lv left.”
* If the money **IS NOT sufficient**:
  * “You'll need {Insufficient funds} lv more.”

The result must be **formatted up to the second symbol** after the decimal point.

## Sample Input and Output

| Input                                               | Output         | Comments                                                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------------------------------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>500<br>3<br>2.5<br>0.5<br>0.7<br>7.80<br>100</p> | 25.60 lv left. | <p><strong>Floor area</strong> → 3 * 2.5 = <strong>7.5</strong><br><strong>Tile area</strong> → 0.5 * 0.7 / 2 = <strong>0.175</strong><br><strong>Needed tiles</strong> → 7.5 / 0.175 = 42.857… = <strong>43 + 5 spare tiles</strong> = <strong>48</strong><br><strong>Total amount</strong> → 48 * 7.8 + 100 (workman) = <strong>474.4</strong><br><strong>474.4 &#x3C; 500</strong> → <strong>25.60 lv left</strong></p> |

| Input                                                       | Output                       | Comments                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------------------------------------------------------- | ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>1000<br>5.55<br>8.95<br>0.90<br>0.85<br>13.99<br>321</p> | You'll need 1209.65 lv more. | <p><strong>Floor area</strong> → 5.55 * 8.95 = <strong>49.67249</strong><br><strong>Tile area</strong> → 0.9 * 0.85 / 2 = <strong>0.3825</strong><br><strong>Needed tiles</strong> → 49.67249 / 0.3825 = 129.86… = <strong>130 + 5 spare tiles</strong> = <strong>135</strong><br><strong>Total amount</strong> → 135 * 13.99 + 321 (workman) = <strong>2209.65</strong><br><strong>2209.65 > 1000</strong> → <strong>1209.65 lv are insufficient</strong></p> |

## Hints and Guidelines

The following task requires our problem to accept more input data and to perform a larger number of calculations, despite the fact that the solution is **identical**. Accepting the input data is done in the **familiar way**. Pay attention that the **Input** part of the condition states that all input data must be in **real numbers**, and for that reason we would use **`decimal`** type.

Now that we already have everything for executing the programming logic, we can move to the following part. How can we **calculate** what is the **needed** number of tiles that will be sufficient to cover the entire floor? The requirement is that tiles have **triangular** shape, which can cause confusion, but practically, the task needs just **simple calculations**. We can calculate the **common part of the floor** by the formula for finding rectangle area, as well as the **area of a single tile** using the relevant formula for triangle area.

In order to calculate the **number of tiles** that are needed, **we divide the floor area by the area of a single tile** (we should not forget to add the 5 additional tiles, that were mentioned in the requirements).

| ![](../../../assets/alert-icon.png) | Pay attention that the requirements state that we should round up the number of tiles, obtained upon the division, up to the higher number, and then we should add 5. Find more information about the system functionality that does that: **`Math.Ceiling(…)`**. |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

We can find the end result by **calculating the total amount** that is needed to cover the entire floor, by **summing up the tile price and the price that will be paid to the workman**, that we have from the input data. We can figure out that **the total costs** for tiles can be calculated by **multiplying the number of tiles by the price per tile**. We fill find out whether the amount that we have will be sufficient by comparing the savings (based on the input data) and the total costs.

## Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/517#1](https://judge.softuni.org/Contests/Practice/Index/517#1).