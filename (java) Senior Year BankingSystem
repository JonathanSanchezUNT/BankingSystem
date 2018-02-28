# BankingSystem
public class BankAccount {
	private double balance;
	
	public BankAccount()
	{
		balance = 0;
	}
	public BankAccount(double acctBalance)
	{
		balance = acctBalance;
	}
	public void deposit (double amount)
	{
		balance += amount;
	}
	public void withdraw(double amount)
	{
		balance -= amount;
	}
	public double getBalance()
	{
		return balance;
	}

}

------------------------------------------------------------------------------

	public class CheckingAccount extends BankAccount 
	{ 
	private static final double atmFEE = 2.0; 
	private static final double MIN_BALANCE = 15.0; 
	private static final double OverDraftFee = 30.0;

	public CheckingAccount() 
	{ 
		super();
	}
	public CheckingAccount(double acctBalance) 
	{ 
		super(acctBalance);
	}
	public void otherATMwithdraw(double amount)
	{
		super.withdraw(atmFEE + amount);
	}

	public void withdraw(double amount) 
	{ 
		super.withdraw(amount);
		
		
		if(super.getBalance() < 50)
		{
			super.withdraw(MIN_BALANCE);
		}
		if(super.getBalance() < 0)
		{
			super.withdraw(OverDraftFee);
		}
	}
  }
  
  -----------------------------------------------------------------------------
public class SavingsAccount extends BankAccount{
	
	private double intrestRate;
	
	public SavingsAccount()
	{
		super();
		intrestRate = 0;
	}
	public SavingsAccount(double acctBalance, double Rate)
	{
		super(acctBalance);
		
		intrestRate = Rate;
	}
	public void addIntreset()
	{
		super.deposit(super.getBalance() * intrestRate);
       
	}

}




