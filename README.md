# array2
package task2.array;

public class ArraysWork {
int arr[] = {15,19,6,3,74,84,62,100,20,38,415,3,74,16,15,9,650,67};
public void getRepeatedValues()
{
System.out.println("Duplicate elements in given array: "); 
for(int i = 0; i < arr.length; i++) { 
for(int j = i + 1; j < arr.length; j++) { 
if(arr[i] == arr[j]) 
System.out.println(arr[j]); 
} 
} 
}

public short getSum()
{
int sum=0;
for(int i = 0; i < arr.length; i++) {
sum=sum+arr[i];


}
System.out.println("Sum ="+sum);
return 0;
}

public void getUniqueValues()
{
System.out.println("Unique elements in given array: "); 
int j=0;
for (int i = 0; i < arr.length; i++) {
for ( j = 0; j < i; j++)
if (arr[i] == arr[j])
break;
if (i == j)
System.out.print( arr[i] + " ");
}
}
public static class ArrayMainClass {
public static void main(String[]args) {
ArraysWork mai=new ArraysWork();
mai.getRepeatedValues();
mai.getSum();
mai.getUniqueValues();

}
}
}
