# java-code\

-----------selection sort--------------



public class Main
{
 public static void main(String []args){
        //System.out.println("Hello World");
        int[] arr = {43,34,5,65,54,34,345,65,12,89};
         int min=0,ind=0;
        for(int i=0;i<arr.length;i++){
           for(int k=i;k<arr.length-1;k++){
               min=arr[k];
                if(min>arr[k+1]){
                    min=arr[k+1];
                    ind=k+1;
                }
           }
           int t=arr[i];
                arr[i]=min;
                arr[ind]=t;
                
        }
        for(int i=0;i<arr.length;i++){
            System.out.print(arr[i]+" ");
        }
     }
}
