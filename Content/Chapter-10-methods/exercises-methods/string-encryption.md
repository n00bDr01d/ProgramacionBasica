# Problem: String Encryption

Write a method **`Encrypt(char letter)`**, which encrypts a given letter in the following way:

* It takes the first and the last digit from the ASCII code of the letter and concatenates them into a string, which will represent the result.
* In the beginning of the string, which represents the result, we will insert the symbol which matches the following condition:
  * ASCII code of the letter + the last digit of the ASCII code of the letter.
* After that in the end of the string, which represents the result, you concatenate the character which matches the following condition:
  * ASCII code of the letter - the first digit of the ASCII code of the letter.
* The method should return the encrypted string.

Example:

* j → **p16i**
  * ASCII code of **j** is **106** → First digit – **1**, last digit – **6**.
  * We concatenate the first and the last digit → **16**.
  * At **the beginning** of the string, which represents the result, concatenate the symbol, which you get from the sum of the ASCII code + the last digit → 106 + 6 → 112 → **p**.
  * At **the end** of the string, which represents the result, concatenate the symbol, which you get from subtracting the ASCII code – the first digit → 106 - 1 → 105 → **i**.

Using the method shown above, write a program which takes **a sequence of characters**, **encrypts them** and prints the result on one line.

The input data will always be valid. The Main method must read the data given by the user – an integer **`n`**, followed by a character for each of the following **`n`** lines.

Encrypt the symbols and add them to the encrypted string. In the end, as a result, you must print **an encrypted string** as in the following example.

Example:

* S, o, f, t, U, n, i → V83Kp11nh12ez16sZ85Mn10mn15h

## Sample Input and Output

| Input                                       | Output                       |
| ------------------------------------------- | ---------------------------- |
| <p>7<br>S<br>o<br>f<br>t<br>U<br>n<br>i</p> | V83Kp11nh12ez16sZ85Mn10mn15h |

| Input                                       | Output                        |
| ------------------------------------------- | ----------------------------- |
| <p>7<br>B<br>i<br>r<br>a<br>H<br>a<br>x</p> | H66\<n15hv14qh97XJ72Ah97xx10w |

## Hints and Guidelines

Firstly, we will give a value of **`string.Empty`** to the **`string`**, which will keep the result. We must recur a loop **`n`** times, so that in each iteration we will add the encrypted symbol to the result string.

In order to find the first and the last digit of the ASCII code, we will use the same algorithm that we used to solve "Integer to Base".

## Testing in the Judge System

Test your solution here: [https://judge.softuni.org/Contests/Practice/Index/594#14](https://judge.softuni.org/Contests/Practice/Index/594#14).
