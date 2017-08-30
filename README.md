/*# java-retirement-calculator-v1
Exercise in learning Java - Retirement Calculator
*/
/*
*Create a program that pulls the current year from
*the computer in order to answer the question: "How
*many more years before I can retire?
 */
package java_retirementcalculator;
import java.util.Scanner;
import java.time.Year;
//import java.time.YearMonth;
//import java.util.Calendar;
//import java.time.LocalDate;
/**
 *
 * @author Paterson4
 */
public class Java_retirementCalculator {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // What is your age?  36
        // At what age would you like to retire?  60
        // You have 24 years left until you can retire.
        // It's 2017, so you can retire in 2041.
        
        Scanner i = new Scanner(System.in);
        
        String age;
        System.out.print("What is your age? ");
        age = i.next();
        
        String retire;
        System.out.print("At what age would you like to retire? ");
        retire = i.next();
        
        Integer a = Integer.valueOf(age);
        Integer r = Integer.valueOf(retire);
        //Integer y = Year.now();
        
        System.out.println("You have "+(r-a)+" years left before you can retire.");
        
        int y;
        y = Year.now().getValue();
        
        //System.out.println(y);
        
        System.out.println("It is "+y+", so you can retire in " + (y + (r-a))+"."); 
    }
    
}
