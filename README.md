# selection_sort
package elclipse;
import java.util.*;
public class selectionsort {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {4,9,5,7,2,8,6,2,78,564,};
		int n=a.length-1;
		int min,temp=0;
		 for(int i=0;i<n;i++) {
			 min=i;                             ///taking first element as minimum
			 for(int j=i;j<n;j++) {
				 if(a[j]<a[min]) {                  //comparing elements
					 min=j;
				 }
			 }
			  temp=a[i];                        ///swappint element with smaller element.
			  a[i]=a[min];
			  a[min]=temp;
		 }
		
		 System.out.print(Arrays.toString(a));
	}

}
