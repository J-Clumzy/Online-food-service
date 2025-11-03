[orca_share_media1762155240429_7391014773553693784.java](https://github.com/user-attachments/files/23297741/orca_share_media1762155240429_7391014773553693784.java)

package food.delivery;

import java.util.Scanner;



public class FoodDelivery {
	public static void main(String[] args) {
		
		
		Scanner sc = new Scanner (System. in);
				System.out.println("_______________________________________________");
					System.out.println("");
					
	System.out.println("Greatings welcome to our online food service!");
	
		System.out.println("_______________________________________________");
	
			System.out.println("Before we get started");
					System.out.println("");
		     System.out.println("Do you have an account? (yes/no):");
        String MainAccount = sc.nextLine().toLowerCase();

        String name = "";
        String address = "";
           String Pick = "";
           
        if (MainAccount.equals("yes")) {
            System.out.println("");
            System.out.println("---------------");
            System.out.println("Great!");
            System.out.println("---------------");
            System.out.println("");
         System.out.println("Enter your name:");
            name = sc.nextLine();
            System.out.println("Enter your address:");
            address = sc.nextLine();
            System.out.println("Pick two numbers (Burger) =1 (Fries) = 2 (Cola) = 3");
            Pick = sc.nextLine();
        } else {
		
		System.out.println("Create an Account Name: ");
		
		name = sc.nextLine();
		
		System.out.println("Account Address: ");
		
		 address = sc.nextLine();
		 
			System.out.println("---------------");
		System.out.println("Account:" + name + "@gmail.com");
					System.out.println("---------------");
		System.out.println("");
		
		System.out.println("---------------");
		
	System.out.println("Address:" + address);	
	
	System.out.println("---------------");
	
	


		System.out.println("Select a number");System.out.println("");
		System.out.println("(1,2,3)");
		System.out.println("");
		System.out.println("Select a secondary number");
	}	
		int choose = Integer.parseInt(sc.next());
		sc.nextLine();
		boolean run = true;
		double total = 0;
		while (run){
		    switch (choose){
		        case 1:
		        System.out.println ("Burger (1)" );
		        
		        System.out.print("How many?");
		        	
  int quantity = Integer.parseInt(sc.next());
		        total += 25 * quantity;
		        
		        break;
		
		    case 2:
		    System.out.println("Fries (2)");
		    
		   System.out.println("How many? =");
		    quantity = sc.nextInt();
		    total += 82 *  quantity;
		    
		    break;
		    
		    case 3: 
		    System.out.println("Cola (3)"); 
		    System.out.println ("How many? =");
		    quantity = sc.nextInt();
		    total += 60 * quantity;
		    
		    break;
		    }
		    System.out.print("Want to add more? (yes/no)");
		    String response = sc.next().toLowerCase();
		    if (response.equals( "yes")){
		        System.out.println("Pick (1) (2) (3)");
		        
		        choose = sc.nextInt();
		    }else{
		        run = false;
		    }
		}
		
		System.out.println("Mr = " + name);
		
		System.out.println("That would be = " + total + "" + "In overall");
		
		System.out.println("Live in = " + address + " Order would arrive shortly");
		
	

		
	}
}
