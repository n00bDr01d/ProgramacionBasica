# Exercises: Methods

In order to learn in practice what we have learned about methods we will **solve a few problems**, in which it will be required to **write methods** with certain functionality and after that to invoke them by passing them data, read from the console.

## What We Learned in This Chapter?

Before starting, let's review what we have learned about the **methods in C#**:

* We learned that the **purpose** of methods is to **split** big programs with a lot of lines of code into smaller, shorter tasks.
* We introduced ourselves with the **structure** of methods, how to **declare** them and **invoke** them by their name.
* We went over examples for methods with **parameters** and how to use them in our program.
* We learned what **signature** and **return value** of a method is and also what is the purpose of the operator `return`.
* We introduced ourselves with the **good practice** when working with methods, how to name them and their parameters, how to format code, etc.

### Defining a Method

This is how we **define a method**, which takes a **parameter** and **returns** a value:

```csharp
static double CircleArea(double radius)
{
    return Math.PI * radius * radius;
}
```

### Invoking a Method

This is how we **invoke a method**, pass a parameter value (**argument**) for the invocation and process the returned value:

```csharp
Console.WriteLine("a = {0}, area = {1}", 5.33, CircleArea(5.33));
// a = 5.33, area = 89.2491915365671

Console.WriteLine("a = {0}, area = {1}", 9.999, CircleArea(9.999));
// a = 9.999, area = 314.0964366475
```

## The Exercises

We will work on the following exercises:

* [Problem: "Hello, Name!"](hello-name.md)
* [Problem: Min Method](min-method.md)
* [Problem: String Repeater](string-repeater.md)
* [Problem: N-th Digit](nth-digit.md)
* [Problem: Integer to Base](integer-to-base.md)
* [Problem: Notifications](notifications.md)
* [Problem: Numbers to Words](numbers-to-words.md)
* [Problem: String Encryption](string-encryption.md)
