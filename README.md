# JavaCode
My Java Programs
/*
    Programmer: CLERENCE MAKUNGU
    Intructor: PHYELA MBEWE
    Program: an m*m matrix
*/
    

import java.util.*; //import the scanner object

public class Matrix
{
    public static void main (String [] args)
    {
        Scanner scan = new Scanner(System.in); //use the scanner object
        System.out.println("Please enter the desired size of your matrix:");
        
        int m = scan.nextInt(); //gets input from user
        int R = 1;
        
        System.out.println("Your matrix is:");

        while ( R < m) //outer loops begins
            {
            for (int C = 1; C <= m; C++) //inner loops begins
            {
                if (C == 1){
                    System.out.print("1"); //prints 1 when Column is on #1
                    }
                else if (R == C){
                    System.out.print("1"); //prints 1 when Row # equal to Column #
                    }
                else if (C == m) {
                    System.out.print("1"); //prints 1 when Column equal to user input
                    }
                else {
                    System.out.print("0"); //prints 0 when none of the above are true
                    } // end of inner loop
                
            }
        System.out.println(" "); //next line
        R++; //increments the outer loop
        } // end of outer loop
        
    }
}
