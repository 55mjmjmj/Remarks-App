import java.util.Scanner;

public class RemarksApp 
{
public static void main(String[] args) 
{
	Scanner scan = new Scanner (System.in);
	System.out.println("Enter the marks");
	int marks = scan.nextInt();
	int cgpa = marks/10;
	System.out.println("Your cgpa is: "+cgpa);
	printRemarks(cgpa);
}
	public static void printRemarks(int cgpa)
	{
		switch (cgpa)
		{
		case 10:
		case 9:
		case 8: System.out.println("Excellent");
		break;
		case 7:
		case 6: System.out.println("Good");
		break;
		case 5: System.out.println("ok");
		break;
		case 4:
		case 3:
		case 2: System.out.println("Poor");
		break;
		case 1:
		case 0: System.out.println("Get lost");
		break;
		default: System.out.println("invalid");
		}
	}
}
