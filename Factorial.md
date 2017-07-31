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
