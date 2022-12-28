# 4.2. More Complex Conditions – Exam Problems

The previous chapter introduced you to **nested conditions** in C#. Via nested conditions, the program logic in a particular application can be represented using **`if` conditional statements** that are nested one into another. We also explained the **`switch-case`** conditional statement that allows selecting from a list of options.

Now we are going to solve some **practical exercises** and make sure we have in-depth understanding of the material, by discussing a number of more complex problems that had been given to students on exams.

## More Complex Conditions – Quick Review

Before moving to the problems, let's first recall what **nested conditions** are.

### Nested Conditions

```csharp
if (condition1)
{
    if (condition2)
        // body; 
    else
        // body;
}
```

| ![](../assets/alert-icon.png) | Remember that it is not a good practice to write deeply nested conditional statements (with more than three levels of nesting). Avoid nesting of more than three conditional statements inside one another. This complicates the code and makes its reading and understanding difficult. |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

### Switch-Case Conditions

When the program operation depends on the value of a variable, instead of doing consecutive checks with multiple `if-else` blocks, we can use the `switch-case` conditional statement.

```csharp
switch (selector)
{
    case value1
        statement;
        break;
    case value2
        statement;
        break;
    default
        statement;
        break;
}
```

The structure consists of a `selector` (an expression that calculates a particular value) + multiple `case` labels followed by commands, ending in a `break`. The selector type can be an integer, string or enumeration (enum).

## Exam Problems

Now, after we refreshed our knowledge on how to **use and nest conditional statements** in order to implement more complex conditions and program logic, let's solve some **exam problems**:

* [Problem: On Time for the Exam](on-time-for-the-exam.md)
* [Problem: Trip](trip.md)
* [Problem: Operations with Numbers](operations.md)
* [Problem: Game Tickets](match-tickets.md)
* [Problem: Hotel Room](hotel-room.md)