# primecountinarray
import java.util.*;
class PrineCount
 {
    public static void main(String args[]) 
    {
       
        int i, j,n,a;
        int count=0;
       
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter size of an array:");
        n = sc.nextInt();
        int arr[]= new int[n];
        System.out.print("Enter array elements:");
        for (i = 0; i < n; i++) 
        {
            arr[i] = sc.nextInt();
        }

        for (i = 0; i < n; i++) 
        {
          a=1;
          for(j=2;j<arr[i];j++)
          {
            
            if (arr[i] % j == 0) 
            {
                    a = 0;
                    break;
                }
               
            }
            if (a== 1) 
            {
              count++;
            }
        }
       System.out.print(" " + count);
    }
}
