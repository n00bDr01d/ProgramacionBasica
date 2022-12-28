# Problem: Logistics

You are responsible for the logistics various types of cargo. **Depending on the weight** of each cargo, you need a **different vehicle**, and this will cost a **different price per ton**:

* Up to **3 tons** – a **minibus** (200 USD per ton).
* From **over 3 and up to 11 tons** – **truck** (175 USD per ton).
* **Over 11 tons – train** (120 USD per ton).

Your task is to calculate **the average price per ton of the cargo**, and also **what percentage of the cargo is transported in each vehicle**.

## Input Data

From the console we must read a **sequence of numbers**, each on a separate line:

* **First line**: **count of cargo** for transportation – **integer** in the range of \[**1 … 1000**].
* On the next lines we pass **the tonnage of the current cargo** – **integer** in the range of \[**1 … 1000**].

## Output Data

Print on the console **4 lines**, as follows:

* **Line #1** – **the average price per ton of the cargo** (rounded up to the second digit after the decimal point).
* **Line #2** – **percentage** of the cargo, carried by **minibus** (between 0.00% and 100.00%, rounded up to the second digit after the decimal point).
* **Line #3** – **percentage** of the cargo, carried by **truck** (between 0.00% and 100.00%).
* **Line #4** – **percentage** of the cargo, carried by **train** (between 0.00% and 100.00%).

## Sample Input and Output

| **Input**                     | **Output**                                  | **Explanations**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ----------------------------- | ------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>4<br>1<br>5<br>16<br>3</p> | <p>143.80<br>16.00%<br>20.00%<br>64.00%</p> | <p>By minibus you transport two of the cargo 1 + 3, total of 4 tons.<br>By truck you transport one of the cargo: 5 tons.<br>By train you transport one of the cargo: 16 tons.<br>Sum of all cargo is: 1 + 5 + 16 + 3 = 25 tons.<br>Percentage of the cargo by minibus: 4/25*100 = 16.00%<br>Percentage of the cargo by truck: 5/25*100 = 20.00%<br>Percentage of the cargo by train: 16/25*100 = 64.00%<br>Average price per ton of carried cargo: (4 * 200 + 5 * 175 + 16 * 120) / 25 = 143.80</p> |

| **Input**                           | **Output**                                 | **Input**                        | **Output**                                |
| ----------------------------------- | ------------------------------------------ | -------------------------------- | ----------------------------------------- |
| <p>5<br>2<br>10<br>20<br>1<br>7</p> | <p>149.38<br>7.50%<br>42.50%<br>50.00%</p> | <p>4<br>53<br>7<br>56<br>999</p> | <p>120.35<br>0.00%<br>0.63%<br>99.37%</p> |

## Hints and Guidelines

First, **we will read the weight of each cargo** and **sum** how much tons are being transported by **minibus**, **truck** and **train**, and we will calculate the **total tons** of the transported cargo. We will calculate **prices for each type of transportation** according to the transported tons and the **total price**. Finally, we will calculate and print **the total average price per ton** and **how much of the cargo is being transported by different types of transport in percentages**.

We declare the needed variables, for example: **`countOfLoads`** – count of the cargos for transportation (we read them from the console), **`sumOfTons`** – sum of the tonnage of all cargos, **`microbusTons`**, **`truckTons`**, **`trainTons`** – variables that keeps the sum of the cargo tonnage, transported by minibus, truck and train.

We still need a **`for` loop** from **`0`** to **`countOfLoads-1`**, to iterate through all cargo types. For each cargo **we read its weight** (in tons) from the console and save it in a variable, for example **`tons`**. We add to the tonnage the sum of all cargo (**`sumOfTons`**) the weight of the current cargo (**`tons`**). Once we have read the weight of the current cargo, **we need to determine which vehicle type will be used** (minibus, truck or train). For this we will need **`if-else`** statements:

* If the value of the variable **`tons`** is **less than 3**, increase the value of **`microbusTons`** by the value of **`tons`**:

```csharp
microbusTons += tons;
```

* Otherwise, if the **`tons`** are **less than 11**, increase **`truckTons`** by **`tons`**.
* If **`tons`** are **more than 11**, increase **`trainTons`** by **`tons`**.

Before we print the output, we need to **calculate the percentage of tons, transported by each vehicle** and the **average price per ton**. For the average price per ton we will declare one more helper variable **`totalPrice`**, in which we will **sum the total price of all transported cargo** (by minibus, truck and train). We will calculate an average price, by dividing **`totalPrice`** of **`sumOfTons`**. You need **to calculate by yourself** the percentages of tons, transported by each vehicle, and print the results, keeping the format specified in the description.

## Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/511#5](https://judge.softuni.org/Contests/Practice/Index/511#5).
