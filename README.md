# Assignment-2-java

import java.util.Scanner; 
public class Marks 
{ 
public static void main(String args[]) 
{ 	
/* This program assumes that the student has 5 subjects, 	
 * thats why I have created the array of size 5. You can 	
 * change this as per the requirement. 	 */ 

int marks[] = new int[5]; 
int i;
float total=0, avg; 
Scanner scanner = new Scanner(System.in); 	
	
for(i=0; i<5; i++) 
{ 
System.out.print("\nEnter Marks of Subjects"+(i+1)+":"); 
marks[i] = scanner.nextInt(); 
total = total + marks[i];
 } 
 
 scanner.close(); 
 
//Calculating average here 

avg = total/5; 
System.out.print("\nThe student average & grade is "+avg+":");  

if(avg>=80) 
{ 
System.out.print("A");
 } 
else if(avg>=60 && avg<80) 
{ 
System.out.print("B"); 
}
else if(avg>=40 && avg<60) 
 { 
 System.out.print("C"); 
 }
 else 
 { 
System.out.print("D"); 
 }
 
  } 
  }

Output:
Enter Marks of Subjects1:80
Enter Marks of Subjects2:70
Enter Marks of Subjects3:90
Enter Marks of Subjects4:85
Enter Marks of Subjects5:95
The student average & grade is 84.0:A
