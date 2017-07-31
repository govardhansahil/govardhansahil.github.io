# Factorial of a Number

`````
import java.io.*;
import java.util.*;

class Factorial
{
	public static void main(String args[])
	{
		int n;
		Scanner s=new Scanner(System.in);
		System.out.println("Enter n value:");
		n=s.nextInt();
		System.out.println("The factorial of "+n+" is "+fact(n));
		
	}
	public static int fact(int num)
	{
		if(num==1 || num==0)
		return 1;
		else
		return num*fact(num-1);
	}
}
`````
# List of Prime Numbers to given number

`````
import java.io.*;
import java.util.*;

class Prime
{
	public static void main(String args[])
	{
		int n;
		Scanner s=new Scanner(System.in);
		System.out.println("Enter number:");
		n=s.nextInt();
		int k=0;
		System.out.println("The Prime numbers until "+n+" are :");
		for(int i=2;i<n;i++)
		{
			for(int j=2;j<i;j++)
			{
				if(i%j==0)
				{
					k++;
					break;
				}
			}
			if(k==0)
			{
				System.out.println(i);
			}
			k=0;
			
		}
	}
}
`````
