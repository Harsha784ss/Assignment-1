1)

import java.util.Scanner;


class Hello{
  public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
    int arr[] = new int[10];
    System.out.println("Enter the array elements:");
    for(int i = 0; i<arr.length; i++){
      arr[i] = sc.nextInt();
    }
    for(int i = 0; i<arr.length-1; i++){
      for(int j=i+1; j<arr.length; j++){
        if(arr[i] == arr[j]){
        System.out.print("Duplicate element in the array:"+arr[i]);
      }
     }
    }
  }
}



2)

import java.util.Scanner;


class Hello{
  public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
    int arr[] = new int[10];
    System.out.println("Enter the array elements:");
    for(int i = 0; i<arr.length; i++){
      arr[i] = sc.nextInt();
    }
    int min = arr[0];
    for(int i = 0; i<arr.length; i++){
      if(arr[i] < min){
       min = arr[i];
      }
    }
    int secmax = arr[0];
   for(int i = 1; i<arr.length; i++){
      if(arr[i] > min && arr[i]< secmax){
        secmax = arr[i];
      }
   }
   System.out.print("Second max:"+secmax);
  }
}

