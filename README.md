# Mycode.dev
import java.util.Scanner;

public class MyCalculator
{
	public static void main(String[] args)
	{
		Scanner sc = new Scanner(System.in);
		
		System.out.print("Enter first number: ");
		int a = sc.nextInt();
		
		System.out.print("Enter second number: ");
		int b = sc.nextInt();
		
		System.out.print("Choose operation: ");
		System.out.println("\n1: Add\n2: Subtract\n3: Multiply\n4: Divide ");
		System.out.print("Enter your choice (1-4): ");
		int sol = sc.nextInt();
		
		switch(sol)
		{
			case 1:
				System.out.println("Result: " + (a+b));
				break;
			case 2:
				System.out.println("Result: " + (a-b));
				break;
			case 3:
				System.out.println("Result: " + (a*b));
				break;
			case 4:
				if (b == 0)
				{
					System.out.println("Undefined (cannot divide by zero)");
				}
				else
				{
					System.out.println("Result: " + (a/b));
				}
				break;
			default:
			System.out.println("Invalid operation selected");
		}
	}
}
