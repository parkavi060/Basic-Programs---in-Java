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

##8.Palindrome Program
````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner scan=new Scanner(System.in);
	System.out.println("Enter number:");
	int num=scan.nextInt();
	int rem;
	int s=0;
	int originalNumber=num;
	while(num!=0){
	    rem=num%10;
	    s=s*10+rem;
	    num/=10;
	}
	if(s==originalNumber) System.out.println("It is a Palindreome");
	else System.out.println("It is not palindreome");
}
}
````

##9.To check if it is a vowel or not.
````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner scan=new Scanner(System.in);
	System.out.println("Enter a character:");
	char c=Character.toLowerCase(scan.next().charAt(0));
	if(c=='a' || c=='e' || c=='i' || c=='o' || c=='u'){
	    System.out.println("The charecter is a vowel");
	}
	else System.out.println("The charecter is consonent");
}
}
````
##10.To check if a String is palindrome or not..
````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner scan=new Scanner(System.in);
	System.out.println("Enter a string:");
	String str=scan.nextLine();
	String reverse="";
	for(int i=str.length()-1;i>=0;i--){
	    reverse+=str.charAt(i);
	}
	if(str.equals(reverse)) System.out.println("Palindrome string");
	else System.out.println("Not a Palindrome String");

}
}
````

##11.Find maximum difference between the numbers in an array..
````java[]
import java.util.*;
public class Main
{
    public static int maxDifference(int [] arr){
        int maxdiff=0;
        for(int i=0;i<arr.length-1;i++){
            for(int j=i+1;j<arr.length;j++){
                maxdiff=Math.max(maxdiff,arr[j]-arr[i]);
            }
        }
        return maxdiff;
    }
	public static void main(String[] args) {
		int arr[]={2,15,67,8,3,9,45,0};
		System.out.println(maxDifference(arr));
	}
}
````

##12.left rotate the string
````java[]
import java.util.*;
public class Main{
    public static void main(String []args){
        Scanner scan=new Scanner(System.in);
        System.out.println("Enter the string");
        String str=scan.nextLine();
        System.out.println("Enter the no. rotations");
        int k=scan.nextInt();
        System.out.println(leftRotate(str,k));
    }
    public static String leftRotate(String str,int k){
        int n=str.length();
        k%=n;
        return str.substring(k)+str.substring(0,k);
    }
    
}
````
##13.Perfect number
````java[]
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    int num=28;
	    int sum=0;
	    System.out.println("The factors are");
	    for(int i=1;i<num;i++){
	        if(num%i==0){
	            System.out.print(i+" ");
	            sum+=i;
	        }
	    }
	    System.out.println();
	    System.out.println("The sum is"+sum);
	    if(sum==num) System.out.println("Answer: It is a prefect number");
	    else System.out.println("Answer: It is not a perfect number");
	   
		
	}
}

````
