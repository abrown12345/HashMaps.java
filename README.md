# HashMaps.java
import java.util.HashMap;
import java.util.Scanner;

public class HashMaps {

	public static void main(String[] args) {
		Scanner userInput= new Scanner(System.in);
		HashMap<String, String> model = new HashMap<>();

		//.put adds items to the hash map
		model.put("Hyundai", "Sonata");
		model.put("Honda", "Civic");
		model.put("Nissan", "Sentra");
		model.put("Dodge", "Ram");
		System.out.println("What car (model) are you looking for?");
		String key= userInput.nextLine();
		String value= model.get(key);
		if (value== null) {
			System.out.println("Sorry, we cannot help you.");
		}
		else 
		{
			System.out.printf("Oh so you're looking for a %s?" + " ", value); 
			System.out.printf("Our %s selection is right over here...", key);
		}
		}
	}
