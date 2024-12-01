# babagsak-ka-ba?

import java.util.*;
public class Main
{
    public static void main(String[] args) {
        double prelim, midterm, prefinals;
        double grade;
        double passingGrade = 75;
        double remainingWeight = 0.40; 
        
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter prelim grade: ");
        prelim = scanner.nextDouble();
        System.out.print("Enter midterm grade: ");
        midterm = scanner.nextDouble();
        System.out.print("Enter prefinals grade: ");
        prefinals = scanner.nextDouble();
        
        
        grade = (prelim * 0.20) + (midterm * 0.20) + (prefinals * 0.20);
        
        
        double needToPass = (passingGrade - grade) / remainingWeight;
        
        System.out.println("Current Grade: " + grade);
        System.out.println("Passing grade is " + passingGrade +
                           ". You need at least " +  needToPass + 
                           " in the finals to pass.");
    }
}
