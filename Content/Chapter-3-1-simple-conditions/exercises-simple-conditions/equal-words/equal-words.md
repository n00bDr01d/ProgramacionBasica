# Problem: Identical Words

Write a program that **inputs two words** and checks if they are the same. Do not make difference between uppercase and lowercase letters. You have to print "**yes**" or "**no**".

## Sample Input and Output

| Input                     | Output |
| ------------------------- | ------ |
| <p>Hello<br>Hello</p>     | yes    |
| <p>SoftUni<br>softuni</p> | yes    |
| <p>Soft<br>Uni</p>        | no     |
| <p>banana<br>lemon</p>    | no     |
| <p>HeLlO<br>hELLo</p>     | yes    |

## Hints and Guidelines

Before comparing the words, turn them into a lowercase to avoid the letter size influence (uppercase / lowercase): **`word = word.ToLower()`**.

## Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/506#10](https://judge.softuni.org/Contests/Practice/Index/506#10).
