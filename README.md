# club-mangement-system-
// SECOND VERSION OF  THE CODE 
import java.util.ArrayList;
// importing the array list class 
// importing collection class to sort the members
// author - nila 
// task- method coder 
// final assignment 
// date= 2021-05-21
import java.util.Collections; 
import java.util.*;
public class MyProgram
{
    
    public static void main(String[] args)
    {
        // code for adding and sorting the member names 
        // Creating an arrayList  to store member names 
        // Adding the members ( 5 people can be added at once 
        // size can be changed later on 
       ArrayList<String > member= new ArrayList<String>();
       System.out.println("__________________________");
       System.out.println(" Adding Members");
       System.out.println("__________________________");
        Scanner order= new Scanner (System.in);
        
         for ( int i=0;i<5; i++)
         {
             System.out.println("Enter the name of the member:");
             String name= order.nextLine();
             member.add(name);
         } 
         // for loop to display the member's name 
         for ( int m=0; m<5; m++)
         {
             System.out.println(" The member name is, "+ member.get(m));
             
    }
    System.out.println("________________________________");
    System.out.println(" Names in order");
    System.out.println("________________________________");
           // calling sortmember function to sort the members 
           sortmembers(member);
}
    // end of main function 
    
    // adding function  to sort the members alphabetically 
    public static void sortmembers(ArrayList<String> member)
    {
    
        // code for sorting the names alphabetically. 
        Collections.sort(member);
        //  for loop to display the names alphabetically 
        for ( int k=0; k<5; k++)
        {
        System.out.println(" Names that is sorted:"+member.get(k));
        
        }
        
    }
}
