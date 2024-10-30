import java.util.Arrays;


public class ReverseArray 
{
    
    public static void main(String[] args) 
    {
        
        int[] array = {10, 12, 13, 14, 15}; 
        System.out.println("Original array: " + Arrays.toString(array));

        reverseArray(array);
        System.out.println("Reverse array: " + Arrays.toString(array));
    }

    public static void reverseArray(int[] arr)
    {
        int left = 0;   
        int right = arr.length - 1;   

        while (left < right) 
        {
            int temp = arr[left];
            arr[left] = arr[right];
            arr[right] = temp;

            left++;
            right--;
        }
    }
}

