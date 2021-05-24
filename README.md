import java.util.ArrayList;
import java.util.Iterator;

  
public class Jala {
	public static void main(String[] args){
		//arraylist created with 10 elements
		ArrayList<String> arraylist = new ArrayList<String>(10);
		arraylist.add("Sai");
		arraylist.add("Yeshwanth");
		arraylist.add("Reddy");
		arraylist.add("Bandi");
		arraylist.add("Yesh");
		arraylist.add("Jala");
		arraylist.add("Java");
		arraylist.add("Python");
		arraylist.add("C++");
		arraylist.add("PHP");
		
		//adding an element to array list
		System.out.println("Adding new element: C");
		arraylist.add("C");
		
		//iterating through iterator operator
		Iterator<String> it = arraylist.iterator();
		System.out.println("Iterating.....");
		while(it.hasNext())
		{
			System.out.println(it.next());
		}
		
		//Adding an element at a specific index
		System.out.println("Adding an element at a specific index: 5");
		arraylist.add(5,"C#");
		
		//removing element 
		System.out.println("Removing an element named C:");
		arraylist.remove("C");
		
		//removing element at particular index
		System.out.println("Removing element at index 6:");
		arraylist.remove(5);
		
		//updating an element at particular index
		System.out.println("Updating an element at particular index 3:");
		arraylist.set(3,"John");
		
		//checking a particular string is present at index
		System.out.println("Element is present at index : "+arraylist.indexOf("Sai"));
		
		//getting element at a particular index
		System.out.println("Getting a particular index element 5");
		arraylist.get(5);
		
		//size of arraylist
		System.out.println("The size of arraylist is : "+arraylist.size());
		
		//element present or not
		System.out.println("Element present or not: "+arraylist.contains("Yesh"));
		
		//remove all elements
		System.out.println("Removing!!!!!");
		arraylist.removeAll(arraylist);
		System.out.println("All elements removed Bye!!!!!!");
	}
}
