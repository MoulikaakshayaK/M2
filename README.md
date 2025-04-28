## NAME : MOULIKAAKSHAYA K
# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
  int m,n,i;
  scanf("%d %d",&m,&n);
  for(i=m;i<=n;i++)
  {
    if(i%2==0)
        printf("%d ",i);
  }
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/cc40ca68-e15c-4a95-a857-5984aa1fb5e0)


## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n,i,j;
    scanf("%d",&n);
    for(i=n;i>=1;--i)
    {
        for(j=1;j<=n-i+1;++j)
        {
            printf("%d",i);
        }
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/975c88ca-1e5e-48ea-9a08-1584fc9485bb)



## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include<stdio.h>
int sum(int,int);
int sub(int,int);
int main()
{
    int a,b,w,s;
    scanf("%d %d",&a,&b);
    w=sum(a,b);
    s=sub(a,b);
    printf("Addition: %d \n", w);
    printf("Subtraction: %d  ", s);
    return 0;
}
int sum(int x,int y)
{
    int z;
    z=x+y;
    return z;
}
int sub( int x, int y)
{
    int s;
    s=x-y;
    return s;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/aefeabae-d393-4c15-8bf6-dd110aa92f94)



## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    int n, sum = 0;
    scanf("%d", &n);
    
    for (int i = 1; i <= n * 2; i += 2) 
    {
        printf("%d ", i);
        sum += i;
    }

    printf("\n%d\n", sum);
    
    return 0;
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/983ab3d0-927a-4b75-91fd-c21d5a63dd7f)



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
int factorial(int n)
{
    int fact = 1;
    for(int i = 1; i <= n; i++) 
    {
        fact = fact * i;
    }
    return fact;
}

int main() {
    int number, result;
    printf("Enter a positive integer: ");
    scanf("%d", &number);
    if (number < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        result = factorial(number); 
        printf("Factorial of %d is %d\n", number, result);
    }

    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/4664f3a8-1609-49ae-a0d5-c600b63e70c3)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
