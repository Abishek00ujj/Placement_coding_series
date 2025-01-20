##  Sort 0 1

#Problem statement
You have been given an integer array/list(ARR) of size N that contains only integers, 0 and 1. Write a function to sort this array/list. Think of a solution which scans the array/list only once and don't require use of an extra array/list.

Note:
You need to change in the given array/list itself. Hence, no need to return or print anything. 
Detailed explanation ( Input/output format, Notes, Images )
Constraints :
1 <= t <= 10^2
0 <= N <= 10^5
Time Limit: 1 sec
Sample Input 1:
1
7
0 1 1 0 1 0 1
Sample Output 1:
0 0 0 1 1 1 1
Sample Input 2:
2
8
1 0 1 1 0 1 0 1
5
0 1 0 1 0
Sample Output 2:
0 0 0 1 1 1 1 1
0 0 0 1 1 

##DUTCH FLAG ALGO


``` java
public class Solution {  

    public static void sortZeroesAndOne(int[] arr) {
        int low=0;
        int high=arr.length-1;
        while(low<high)
        {
            if(arr[low]==0)
            {
                low++;
            }
            else
            {
                int tmp=arr[low];
                arr[low]=arr[high];
                arr[high]=tmp;
                high--;
            }
        }
    }
}

```
![image](https://github.com/user-attachments/assets/c65fe665-37c0-4f7e-95ba-9c874f03b92a)
