package bank;
import java.util.Scanner;

public class SavingsAccount {
	static int balance;
	  static int withdrawal;
	  static int deposit;
	  
	  public SavingsAccount(int initialBalance){
	    balance = initialBalance;
	  }
	  public static int withdrawalAmount(int A){
	    withdrawal = A;
	    if(balance>=withdrawal) {
	    	System.out.println("You just withdrew $" 
	    		    + withdrawal);
	    }
		return A;
	  } 
	  public static int depositAmount(int B){
	    deposit = B;
	    System.out.println("You just deposited $" 
	    + deposit);
		return B;
	  }
	  public static void finalBalanceAfterWithdrawal(){
	    if(balance>=withdrawal) {
	    	int a = balance - withdrawal;
		    balance = a;
		    System.out.println("Your balance is $" + balance);
	    }else {
	    	System.out.println("Sorry!You don't have enough balance in your account left.");
	    }
	  }
	  public static void finalBalanceAfterDeposit(){
	    int b = balance + deposit;
	    balance = b;
	    System.out.println("Your balance is $" + balance);
	  }
	  public static void greetings(){
		  System.out.println("Hello! Welcome to your Savings Account.");
		    System.out.println("Press '1', to check your account balance.");
		    System.out.println("Press '2', to withdraw money from your account.");
		    System.out.println("Press '3', to deposit money in your account.");
		    Scanner sc = new Scanner(System.in);
			int action = sc.nextInt();
			usersAction(action);
	  }
	  public static void usersAction(int action) {
		  int savings = balance;
		  try {
				if(action==1) {
					System.out.println("Your balance is $"+savings);
				}else if(action==2) {
					System.out.println("Please enter the amount you want to withdraw: ");
					Scanner sc1 =  new Scanner(System.in);
					int amountW1 = sc1.nextInt();
					int w1 =  withdrawalAmount(amountW1);
					finalBalanceAfterWithdrawal();
				}else if(action==3) {
					System.out.println("Please enter the amount you want to deposit: ");
					Scanner sc2 =  new Scanner(System.in);
					int amountD1 = sc2.nextInt();
					int d1 = depositAmount(amountD1);
					finalBalanceAfterDeposit();
				}else {
					System.out.println("Error! You pressed the wrong button.");
				}
			}
			catch(Exception e){
				System.out.println("Error!");
			}   
	  }
	  
	  public static void main(String[] args){
		
	    SavingsAccount savings = new SavingsAccount(2000);
	    
	    greetings();

		System.out.println("To continue, Press '0'.");
		System.out.println("To exit, Press '9'.");
	    Scanner sc3 = new Scanner(System.in);
	    int action1 = sc3.nextInt();
	    if(action1==0) {
	    	greetings();
	    	System.out.println("Thanks for banking with us. Have a good day.");
	    }if(action1==9) {
	    	System.out.println("Thanks for banking with us. Have a good day.");
	    }else {
	    	
	    }
		
	  }
}
