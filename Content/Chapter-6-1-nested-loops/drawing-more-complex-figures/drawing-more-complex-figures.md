# Exercises: Drawing Figures

Let's look at how to **draw figures** using **nested loops** with more complex logic, for which we need to think more before coding.

## Video: Chapter Summary

Watch this video to review what we learned in this chapter: [https://youtu.be/tj4s3BOijO4](https://youtu.be/tj4s3BOijO4).

## What We Learned in This Chapter?

Before starting, let's review what we learned in this chapter.

We became acquainted with the `new string` constructor:

```csharp
string printMe = new string('*', 5);
```

We learned to draw figures with nested `for` loops:

```csharp
for (var r = 1; r <= 5; r++)
{
   Console.Write("*");
   for (var c = 1; c < 5; c++)
      Console.Write(" *");
   Console.WriteLine();
}
```

## The Problems

We will work on the following set of practical problems:

* [Problem: Rhombus of Stars](../nested-loops/example-rhombus-of-stars.md)
* [Problem: Christmas Tree](../nested-loops/example-christmas-tree.md)
* [Problem: Sunglasses](sunglasses/sunglasses.md)
* [Problem: House](house/house.md)
* [Problem: Diamond](diamond/diamond.md)
