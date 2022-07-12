# Linear-Search
import java.util.Scanner;
public class SearchingTech {
    public static void main(String[] args) {
    int[] A = {23, 34, 32, 12, 13, 15};
        int i, temp = 0;
        System.out.print("Elements in the array list are: ");
        for(i=0;i<A.length;i++)
            System.out.print(A[i]+" ");
        System.out.print("\nEnter the element you want to get search: ");
        Scanner sc = new Scanner(System.in);
        int item = sc.nextInt();
        for (i = 0; i < A.length; i++) {
            if (A[i] == item) {
                System.out.println("element is found at " + i);
                temp = temp + 1;
            }
        }
        if (temp == 0)
            System.out.println("Element is not found.");
    }
}
