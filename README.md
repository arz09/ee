package ve_no;

import java.util.ArrayList;
import java.util.Date;
import java.util.Scanner;

public class ve_da {

	public static void main(String[] args) {
		Scanner key=new Scanner(System.in);
		ArrayList<String>vn=new ArrayList<String>();
        ArrayList<String>date=new ArrayList<String>();
        
        while(true)
        {
        	System.out.println("1.to add the number and date");
        	System.out.println("2.report  "+vn.size());
        	System.out.println("3.exit");
        	
        	int choice=Integer.parseInt(key.nextLine());
        	
        	if(choice==1)
        	{ 
        		System.out.println("enter the vehicle number");
        		String veno=key.nextLine();
        		vn.add(veno);
        		Date d=new Date();
        		String date1=d.toString();
        		date.add(date1);
        		System.out.println("the vehicle number "+veno+"the time is"+date1);
        		
        	}
        	else if(choice==2)
        	{
        		System.out.println("the toll report");
        		for(int i=0;i<vn.size();i++)
        		{
        			System.out.print(vn.get(i)+"  ");
        			System.out.println(date.get(i));
        			
        		}
        	}
    		else if(choice==3)
    		{
    			break;
    				
    		}
    		else
    		{
    			System.out.print("the input is invalid");
    		}
    			
        	}
        
		
		// TODO Auto-gene	rated method stub

	}

}

