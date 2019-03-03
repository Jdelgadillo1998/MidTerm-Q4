# MidTerm-Q4
import java.util.ArrayList;
import java.util.*;



public class Employee {


	public static void printArray(int arr[] ) {
		for (int element: arr) {
			System.out.print(element + " ");
		}
		System.out.println();
	}

	public static void bubbleSort(int arr[]) {
		int length;
		for (int i=1; i<arr.length; i++) {
			for (int j=0; j<arr.length -1; j++) {
				if(arr[j]> arr[j+1]) {
					int temp = arr[j+1];
					arr[j+1] = arr[j];
					arr[j] = temp;
				}
			}

		}
	}

	public static void main(String[] args) {
		names();
		title();
		wages();


	}
	public static void wages() {
		int[] wages = {20000,45000,80000,24000,16000};
		bubbleSort(wages);
		printArray(wages);
	}
	public static void names() {
		String[] name = {"Steve", "Eric", "Simon", "Jacob"};
		System.out.println(Arrays.toString(name));
	}
	public static void title() {
		String[] name = {"Plumber", "Mechanic", "Teacher", "Doctor"};
		System.out.println(Arrays.toString(name));
	}
}
