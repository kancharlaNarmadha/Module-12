
# EX 12A Java TreeMap
## DATE:
## AIM:
To write a Java program to get all keys from the given a Tree Map.


Note:

Student details are stored in a file "student.txt" using Serialization.

Create a class Studentinfo that implements Serializable interface to make its object serialized.

Initialize transient for dept,,rollno














## Algorithm

1.Import required classes and define the main class Exa.

2.Create a TreeMap to store key-value pairs of strings.

3.Read key-value pairs from the user and insert them into the map using put().

4.Get the set of keys from the map using keySet().

5.Iterate over the key set and print each key.








## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```
import java.util.*;  
public class Exa {  
   public static void main(String args[]){  

   TreeMap<String,String> tree_map1=new TreeMap<String,String>();      
  Scanner sc=new Scanner(System.in);
   int size=sc.nextInt();
   for(int i=0;i<size;i++)
   {
      String n1 = sc.next();
      String s1= sc.next();
       
   	  tree_map1.put(n1,s1);  
   }
    
 Set<String> keys = tree_map1.keySet();
        for(String key: keys){
            System.out.println(key);
        }
    }
}

      


            
      
               


    
```

## Output:

![image](https://github.com/user-attachments/assets/19bf2cd4-e554-4aeb-8a7b-427ba18232d6)


## Result:
Thus, the program to implement a Java program using TreeMap to store data and display only the keys has been successfully executed.








