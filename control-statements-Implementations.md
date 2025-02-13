## 01.Simple If Statement - Check if a number is positive. 
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
