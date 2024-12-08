# is-Ascending-
import java.util.Scanner;

public class Ascending {
    public Ascending() {
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the size of array: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter the elements of array: ");

        for(int i = 0; i < n; ++i) {
            arr[i] = sc.nextInt();
        }

        boolean isAscending = true;

        for(int i = 0; i < n; ++i) {
            if (arr[i] > arr[i + 1]) {
                isAscending = false;
            }
        }

        if (isAscending) {
            System.out.println("The array is sorted in Ascending order");
        } else {
            System.out.println("The array is not sorted");
        }

    }
}
