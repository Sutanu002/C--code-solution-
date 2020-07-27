# C--code-solution-
Print Fibonacci Series 
Code :
#include<stdio.h>
#include<conio.h>
int fib(int);
void main()
{
    int n,i;
    printf("Enter the nth term : \n");
    scanf("%d",&n);
   printf("Fibonacci series is : ");
    for(i=0;i<n;i++)
        printf(" %d ",fib(i));
    getch();
}
int fib(int n)
{
    if(n==0)
        return 0;
    if(n==1||n==2)
        return 1;
    else
        return fib(n-1)+fib(n-2);
}

Output :     Enter the n th term :
	        12
                    Fibonacci series is :   0  1  1  2  3  5  8  13  21  34  55  89 
