# Switch-Case Conditional Statement

The **`switch-case`** condition works as a sequence of **`if-else`** blocks. Whenever the work of our program depends on the value of **one variable**, instead of making consecutive conditions with **`if-else`** blocks, we can **use** the conditional **`switch`** statement. It is being used for **choosing between a list of possibilities**. The statement compares a given value with defined constants and depending on the result, it takes an action.

We put **the variable** that we want to **compare**, inside the **brackets after the operator `switch`** and it is called a "**selector**". Here **the type must be comparable** (numbers, strings). **Consecutively**, the program starts **comparing** each **value** that **is found** after the **`case` labels**. Upon a match, the execution of the code from the respective place begins and continues until it reaches the operator **`break`**. In some programming languages (like C and C++) **`break`** might be skipped, in order to execute a code from other **`case`** construction, until it reaches another operator. In C# though, the presence of **`break`** is **mandatory** for **every `case`** that contains a program logic. When **no matches** are **found**, the **`default`** construction is being executed, **if** such **exists**.

```csharp
switch (selector)
{
    case value1:
        construction;
        break;
    case value2:
        construction;
        break;
    case value3:
        construction;
        break;
    …
    default:
        construction;
        break;
}
```

## Video: Switch-Case

Watch the video to learn how to use the switch-case conditional statement: https://youtu.be/mGJOc4xx5Ho.

## Example: Day of the Week

Let's write a program that prints **the day of the week** (in English) depending on the **given number** (1 … 7) or "**Error!**" if an invalid input is given.

### Sample Input and Output

| Input               | Output                            |
| ------------------- | --------------------------------- |
| <p>1<br>7<br>-1</p> | <p>Monday<br>Sunday<br>Error!</p> |

### Solution

![](../../../assets/chapter-4-images/09.Day-of-week-01.png)

| ![](../../../assets/alert-icon.png) | It is a good practice to put at the first place those `case` statements that process the most common situations and leave the `case` constructions processing the more rear situations at the end, before the `default` construction. Another good practice is to arrange the `case` labels in ascending order, regardless of whether they are integral or symbolic. |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

### Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/508#8](https://judge.softuni.org/Contests/Practice/Index/508#8).

## Multiple Labels in Switch-Cases

In **C#** we have the possibility to **use multiple `case`** labels in the `switch-case` coonstruction, when they have to execute **the same code**. This way, when our **program** finds a **match**, it will execute the **next** code, because **after** the respective **`case`** label **there is no code** for execution and a **`break`** operator.

```csharp
switch (selector)
{
    case value1:
    case value2:
    case value3:
        construction;
        break;
    case value4:
    case value5:
        construction;
        break;
    …
    default:
        construction;
        break;
}
```

## Example: Animal Type

Write a program that prints the type of the animal depending on its name:

* dog -> **mammal**
* crocodile, tortoise, snake -> **reptile**
* others -> **unknown**

### Sample Input and Output

| Input    | Output  | Input | Output | Input    | Output  |
| -------- | ------- | ----- | ------ | -------- | ------- |
| tortoise | reptile | dog   | mammal | elephant | unknown |

### Solution

We can solve the task with **`switch`**-**`case`** conditions with multiple labels in the following way:

![](../../../assets/chapter-4-images/10.Animal-type-01.png)

### Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/508#9](https://judge.softuni.org/Contests/Practice/Index/508#9).
