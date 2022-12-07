# BasicCalculator.java
   import java.lang.*;
	 import java.util.*; 	
	   public class Calculator {

			public static void main(String[] args)
			{
			
				double number1, number2;

			    Scanner sc = new Scanner(System.in);
			    
			    System.out.println("Enter the number1 : ");
                number1 = sc.nextDouble();
				
                
                System.out.println("Enter the operator (+,-,*,/,%,^) : ");
				char operator = sc.next().charAt(0);
                
				System.out.print("Enter the number2 : ");
				number2 = sc.nextDouble();
				
				
				double result = 0;
                                
                
				switch (operator) {

				
				case '+':
					result = number1 + number2;
					break;

				case '-':
				    result = number1 - number2;
					break;
				
				case '*':
					result = number1 * number2;
					break;
				
				case '/':
					result = number1 / number2;
					break;
				
				case '%':					
					result = (number1 / number2)*100;				
					break;
				
				case '^':
				    result = Math.pow(number1, number2);
					break;
					
					
				default:

					System.out.println("You enter wrong input");

					break;
				}

				System.out.println();
				
				System.out.println("The final result:");

				System.out.println();

				System.out.println(number1 + " " + operator + " " + number2+ " = " + result);
			
			}
		

	}


