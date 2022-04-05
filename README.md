# Write-a-program-to-generate-a-map-containing-i-i-i-where-i-is-an-integer-from-1-to-n-including-
Use a for loop to iterate i from 1 to n.
package vn.viettuts.baitap;
 
import java.util.HashMap;
import java.util.Map;
import java.util.Scanner;
 
public class Bai03 {
     private static Scanner scanner = new Scanner(System.in);
 
     public static void main(String[] args) {
         System.out.print("Enter positive integer n = ");
         int n = scanner.nextInt();
         
         Map<Integer, Integer> map = new HashMap<Integer, Integer>();
         for (int i = 1; i < n + 1; i++) {
             map.put(i, i * i);
         }
         System.out.println(map);
     }
}
