# Atm_Project
This is  ATM  project of java source code 
import java.util.*;
class ATM
{
	public static void main(String [] args)
	{
        
		int balance=100000,withdraw,deposite;
		Scanner scn=new Scanner(System.in);
		
		System.out.println("Automated Teller Machine");
		System.out.println("1.WITHDRAW");
		System.out.println("2.DEPOSITE");
		System.out.println("3.CHECK BALANCE");
		System.out.println("4.EXIT");
		while(true)
		{
			System.out.println("Automated Teller Machine:");
			System.out.println("Choose for 1 withdraw");
			System.out.println("Choose for 2 Deposite:");
			System.out.println("Choose for 3 check balance");
			System.out.println("Choose for 4 EXIT");
		}
		
	        choice=scn.nextInt();
		
		switch(choice)
		{
			case 1:
			System.out.println("Enter Your Money to be withdraw:");
			withdraw=scn.nextInt();
			if(balance>=withdraw)
			{    
		        balance=balance-withdraw;
				System.out.println("Please Collect Your Money:");
			}
			else
			{
				System.out.println("Insufficient Balance:");
			}
			break;
			
			case 2:
			System.out.println("Enter Your Money Deposite:");
			deposite=scn.nextInt();
			balance=balance+deposite;
			System.out.println("Your Money has been Deposited Successfully:");
			break;
			
			case 3:
			System.out.println("Balance: "+balance);
			break;
			case 4:
			System.exit(0);
		}

		
		
	}
}
