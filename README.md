# Harshad-number-or-not-using-Java

Harshad number or not using Java
Harshad number or not using Java : 
Harshad number is a number or an integer in base 10 which is completely divisible by sum of  its digits.

For better understanding let us consider an example.

Example :

Suppose a number 24 .
Calculate the sum of digits of the number (2 + 4) = 6 .
Check whether the number entered by user is completely divisible by sum of its digits or not.
Below are first few Harshad Numbers represented in base 10 :

1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 18, 20………

In this article, we will create a java program to check whether the number entered by the user is Harshad number or not.

harshed or not in java
Working :
Step 1 : Ask the user to enter an integer.

Step 2 : Declare two variables, one for storing sum of digits and second for storing copy of the original number.

Step 3 : Use a while loop to perform continuous operations till the value of the integer do not becomes 0.

Step 4 : Use a statement to pick the last digit of the integer..

Step 5 : Perform addition and store the result in every iteration. 

Step 6 : Restore the integer value by removing last digit in every iteration of the loop.

Step 7 : Repeat the Steps from 3 to 6 till the integer value do not becomes 0.

Step 8 : Compare that whether the sum of digits of the integer is equal to the given integer or not.

If this gets true , then the given number is Harshad Number.
Else the number is not a Harshad Number. 
 

Harshad number or not in java
Code in Java :
Run
//Java program to check whether a number is harshad number or not
// Online Java Compiler
// Use this editor to write, compile and run your Java code online

public class Main {
    public static void main(String[] args)
	{
		//make a copy of original number
		int n = 47;
		//declare a variable to store sum of digits
		int result = 0;
		//perform logic for calculating sum of digits of a number
		while(n != 0)
		{
			int pick_last = n % 10;
			result = result + pick_last;
			n = n / 10;
		}
		/*use condition to check whether the number entered by  
		user is completely divisible by its sum of digits or not*/
      if(n % result == 0)
      System.out.println("Harshad Number");
          else
        System.out.println("Not a Harshad Number");
}
}
Output :
Enter a number : 18
Harshad Number
Enter a number : 345
Not a Harshad Number
