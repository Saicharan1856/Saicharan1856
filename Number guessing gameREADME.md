- 👋 Hi, I’m @Saicharan1856
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Saicharan1856/Saicharan1856 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import java.util.Scanner;  
  

public class ATMExample  
{  
    
    public static void main(String args[] )  
    {  
        
        int balance = 100000, withdraw, deposit;  
          
        
        Scanner sc = new Scanner(System.in);  
          
        while(true)  
        {  
            System.out.println("Automated Teller Machine");  
            System.out.println("Choose 1 for Withdraw");  
            System.out.println("Choose 2 for Deposit");  
            System.out.println("Choose 3 for Check Balance");  
            System.out.println("Choose 4 for EXIT");  
            System.out.print("Choose the operation you want to perform:");  
              
            
            int choice = sc.nextInt();  
            switch(choice)  
            {  
                case 1:  
        System.out.print("Enter money to be withdrawn:");  
                      
        
        withdraw = sc.nextInt();
        if(balance >= withdraw)  
        {  
            
            balance = balance - withdraw;  
            System.out.println("Please collect your money");  
        }  
        else  
        {  
            
            System.out.println("Insufficient Balance");  
        }  
        System.out.println("");  
        break;  
   
                case 2:  
                      
        System.out.print("Enter money to be deposited:");  
                      
        
        deposit = sc.nextInt();  
                      
        
        balance = balance + deposit;  
        System.out.println("Your Money has been successfully depsited");  
        System.out.println("");  
        break;  
   
                case 3:  
        
        System.out.println("Balance : "+balance);  
        System.out.println("");  
        break;  
   
                case 4:  
        
        System.exit(0);  
            }  
        }  
    }  
}
