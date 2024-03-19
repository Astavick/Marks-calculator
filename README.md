package lecturer_marks;
import java.util.Scanner;
public class MarksCalculator {

    public static void main(String[] args) {
        calculateMarks();
    }

    public static void calculateMarks() {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter marks for Java programming: ");
        int javaMarks = input.nextInt();

        System.out.print("Enter marks for Networking: ");
        int networkingMarks = input.nextInt();

        System.out.print("Enter marks for Maths: ");
        int mathsMarks = input.nextInt();

        int totalMarks = javaMarks + networkingMarks + mathsMarks;
        double average = (double) totalMarks / 3;

        System.out.println("Marks for Java programming is: " + javaMarks);
        System.out.println("Marks for Networking is: " + networkingMarks);
        System.out.println("Marks for Maths is: " + mathsMarks);
        System.out.println("The average is: " + average);
    }
}
