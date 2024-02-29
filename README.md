import java.util.Scanner;
public class calculateAverage {
    public static void main(String[] args) {
        float average =0.0f;
        Scanner sc = new Scanner(System.in);
        
        /*This line declares array Integer Wrapper Object */
        Integer ciel, cie2, cie3;
        /* - Autobox
        * The parsed value of integer constant is converted wrapper  Object */ 
        System.out.println("Enter the score of First Internal:");
        ciel = Integer.parseInt(sc.next());
        System.out.println("Enter the score of Second Internal: ");
        cie2 = Integer.parseInt(sc.next());
        System.out.println("Enter the score of Third Internal: ");
        cie3= Integer.parseInt(sc.next());
        /* Unbox
        * The wrapper Object value is converted into Primitive Data Type */ 
        average = (float) (ciel + cie2 + cie3)/3;
        System.out.println("The average Internal Score is "+average);
        sc.close();
    }
}﻿
OUTPUT:
Enter the score of First Internal: 26
Enter the score of Second Internal: 15
Enter the score of Third Internal: 22
The average Internal Score is 21.
﻿/* This program illustrates Autobox and Unbox of Data Types */ 
import java.util.Scanner;
public class calculateAverage {
  public static void main(String[] args) {
    float sum =0.0f;
    Scanner sc = new Scanner (System.in);
    /*This line declares array Integer Wrapper Object */ 
    Integer cie[] = new Integer [3];
    
    for (int i=0; i< 3; i++) {
      System.out.println("Enter the score of Internal : "+(i+1));
      /* - Autobox
      * The parsed value of integer constant is converted wrapper Object */ 
      cie[i] = Integer.parseInt(sc.next());
      /* Unbox
      * The wrapper Object value is converted into Primitive Data Type */ 
      sum=sum + cie[i];
    }
      System.out.println("The average Internal Score is "+(sum/3));
      sc.close();
    
  }
}
OUTPUT:
Enter the score of Internal : 1
16
Enter the score of Internal : 2
161   38303    0
Enter the score of Internal : 3
21
The average Internal Score is 22.333334


