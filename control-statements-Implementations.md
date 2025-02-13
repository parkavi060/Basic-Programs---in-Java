## 01.Simple If Statement - Check if a number is positive, 02.Check if the number is positive or negative.
````java[]
import java.util.*;

public class Main
{
	public static void main(String[] args) {
		Scanner scan=new Scanner(System.in);
		System.out.println("Enter the element:");
		int num=scan.nextInt();
		if(num<0) System.out.println("Number "+num+" is negative");
		else if(num>0) System.out.println("Number "+num+" is positive");
		else  System.out.println("Number given number is zero");
	}
}
````

##03.If-Else if-Else Statement - Find the largest of three numbers.  
````java[]
import java.util.*;

public class Main
{
	public static void main(String[] args) {
		Scanner scan=new Scanner(System.in);
		System.out.println("Enter the three numbers:");
		int num1=scan.nextInt();
		int num2=scan.nextInt();
		int num3=scan.nextInt();
		if(num1>num2 && num1>num3) System.out.println(num1+" is greatest number.");
		else if(num2>num1 && num2>num3) System.out.println(num2+" is greatest number.");
		else System.out.println(num3+" is greatest number.");
	}
}
````

##04.Nested If-Else Statement - Check whether a year is a leap year or not. 
````java[]
````
