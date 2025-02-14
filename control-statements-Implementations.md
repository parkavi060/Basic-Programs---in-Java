## 01.Simple If Statement - Check if a number is positive, 02.Check if the number is positive or negative,14.Check Positive or Negative Number Using Nested If - Nested condition check for positive or negative. 
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
import java.util.*;

public class Main
{
	public static void main(String[] args) {
		Scanner scan=new Scanner(System.in);
		System.out.println("Enter the three numbers:");
		int year=scan.nextInt();
		if(year%4==0 ||(year%400==0&&year%100!=0)) System.out.println("Leap year");
		else System.out.println("Not Leap year");

	}
}
````

##05.Switch Case - Print the name of a day based on input number (1 to 7). 
````java[]
import java.util.*;

public class Main
{
	public static void main(String[] args) {
		Scanner scan=new Scanner(System.in);
		System.out.println("Enter the number to find the day:");
		int day=scan.nextInt();
		switch(day){
		    case 1:
		    System.out.println("Monday");
		    break;
		    case 2:
		    System.out.println("Tuesday");
		    break;
		    case 3:
		    System.out.println("Wednesday");
		    break;
		    case 4:
		    System.out.println("Thursday");
		    break;
		    case 5:
		    System.out.println("Friday");
		    break;
		    case 6:
		    System.out.println("Saturday");
		    break;
		    case 7:
		    System.out.println("Sunday");
		    break;
		    
		}
		

	}
}
````

##6.Find Grade Using Switch Case - Find grades based on marks. 

````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
		Scanner scan=new Scanner(System.in);
		System.out.println("Enter the mark:");
		int mark=scan.nextInt();
		if(mark<0||mark>100){
		    System.out.println("Invalid mark");
		}
		else{
		    switch(mark/10){
		       case 10:
		            System.out.println("Grade:O");
		            break;
		      case 9:
		            System.out.println("Grade:O");
		            break;
		      case 8:
		            System.out.println("Grade:A+");
		            break;
		      case 7:
		            System.out.println("Grade:A");
		            break;
		      case 6:
		            System.out.println("Grade:B+");
		            break;
		      case 5:
		            System.out.println("Grade:B");
		            break;
		      case 4:
		            System.out.println("Grade:C");
		            break;
		      case 3:
		            System.out.println("Grade:F(Fail)");
		            break;
		    }
		}
	}
}

````

##7.Prime number program
````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner scan=new Scanner(System.in);
	System.out.println("Enter number:");
	int num=scan.nextInt();
	 if(num<=1){
	     System.out.println("Not a prime number");
	 }
	 boolean isPrime=true;
	 for(int i=2;i<=num/2;i++){
	     if(num%i==0) {
	         isPrime=false;
	         break;
	     }
	 }
	 if(isPrime) System.out.println("The number is prime");
	 else System.out.println("The number is not prime");
}
}
````
