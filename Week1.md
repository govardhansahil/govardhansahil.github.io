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
# Roots of Quadratic Equation
`````
import java.io.*;
import java.util.*;

class Quadratic
{
	
	public static void main(String args[])
	{
		int a,b,c,d;
		Scanner s=new Scanner(System.in);
		System.out.print("The Quadratic Equation is of the form ax2+bx+c=0\nPlease enter the values\na=");
		a=s.nextInt();
		System.out.print("\nb=");
		b=s.nextInt();
		System.out.print("\nc=");
		c=s.nextInt();
		System.out.println("The Quadratic Equation entered is "+a+"x2+"+b+"x="+c+"=0");
		d=(b*b)-(4*a*c);
		if(d==0)
		{
			System.out.println("The Roots are Real and Equal");
			double r=(-b+Math.sqrt(d))/(2*a);
			System.out.println(r+"  "+r);
		}
		else if(d>0)
		{
			System.out.println("The Roots are Real and distinct");
			double r1=(-b+Math.sqrt(d))/(2*a);
			double r2=(-b-Math.sqrt(d))/(2*a);
			System.out.println(r1+"  "+r2);
		}
		else if(d<0)
		{
			System.out.println("The Roots are Imaginary");
			double real=(-b)/(2*a);
			double imag=(Math.sqrt(-d))/(2*a);
			System.out.println(real+"+i"+imag+"\n"+real+"-i"+imag);
		}
	}
}
`````
