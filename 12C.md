
# EX 12B Comparable and Comparator Interface
## DATE:
## AIM:
To write a java program to illustrate Comparator using a separate class(Percentage comparator).Read student name and percentage of student).Display in highest percentage to low using comparator.















## Algorithm

1.Define a Student class with name and percentage fields and a constructor.

2.Implement a PercentageComparator class to compare students by percentage in descending order.

3.Read a list of students (name and percentage) from the user and store them in an ArrayList.

4.Sort the student list using Collections.sort() with the custom comparator.

5.Display the sorted list showing percentage and name.








## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```
import java.util.*;

class Student{

	String name;
	float percentage;
	
	Student(String name, float percentage){
		this.name = name;
		this.percentage = percentage;
	}
	
}

class PercentageComparator implements Comparator<Student>{
	public int compare(Student stud1, Student stud2) {
		if(stud1.percentage < stud2.percentage)
			return 1;
		return -1;
	}
}

public class Main{
	
	public static void main(String args[]) {
	
		ArrayList<Student> studList = new ArrayList<Student>();
		Scanner sc=new Scanner(System.in);
		int size=sc.nextInt();
		for(int i=0;i<size;i++)
		{
		    studList.add(new Student(sc.next(), sc.nextInt()));
		}
		
		Comparator<Student> com = new PercentageComparator();
		
		Collections.sort(studList, com);
		
		System.out.println("Avg % --> Name");
		System.out.println("---------------------");
		for(Student stud:studList) {
			System.out.println(stud.percentage + " --> " + stud.name);
		}		
	}	
}

      


            
      
               


    
```

## Output:

![image](https://github.com/user-attachments/assets/bc236ed4-2f35-4167-a059-19dd711deadb)


## Result:
Thus, the program to implement a Java program using Comparator to sort student records based on percentage has been successfully executed.









