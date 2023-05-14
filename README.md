# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:
## Step 1:
Create a function for reversing.
## Step 2:
Get the number from the user.
## Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.
## Step 4:
Recusively call this function to get the reversed number.
## Step 5:
print the reversed number.

## Program:
~~~
Developed by: M Parshwanath
Reg no: 212221230073
~~~
~~~
using System;
namespace Recursive_Function
{
    class Program
    {
        public static int m, reverse = 0;
        public static int Recur(int number)
        {
            
            if (number > 0)
            {
                Program.m = number % 10;
                Program.reverse = Program.reverse * 10 + m;
                number = number / 10;
                return Recur(number);
            }
            return Program.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(Recur(num));
        }
    }
}
~~~
## Output:

![Screenshot 2023-05-14 220557](https://github.com/parsh2004/Recursive-function/assets/95388047/850d035d-2837-4177-b0b8-ae1af883c5cc)

## Result:
Thus the C# program to reverse a number using recursive function is executed successfully.
