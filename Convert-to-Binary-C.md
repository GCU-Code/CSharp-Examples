---
title: LAB 3-32: Convert to Binary
subtitle: CST-105
author: Brent L. Ricks
date: July 8, 2022
subject: Lab
---

# LAB 3-32: Convert to Binary

```csharp
/*
Write a program that takes in a positive integer as input, and outputs a string of 1's and 0's representing the integer in binary. For an integer x, the algorithm is:

As long as x is greater than 0
   Output x % 2 (remainder is either 0 or 1)
   x = x / 2
Note: The above algorithm outputs the 0's and 1's in reverse order.

Ex: If the input is: 6
the output is:011

6 in binary is 110; the algorithm outputs the bits in reverse.
*/

using System;

namespace PracticeLabs
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int x;

            x = Convert.ToInt32(Console.ReadLine());

            while (x > 0)
            {
                Console.Write(x % 2);
                x = x / 2;
            }
            Console.WriteLine();
        }
    }
}
```