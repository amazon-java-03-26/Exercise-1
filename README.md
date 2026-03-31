
📦 Java Exercises – Warehouse 

🧩 Exercise 1 – Create the Class

Create PackageItem.

Do:
	•	Fields:
	•	id (String)
	•	weight (double)
	•	priority (String)
	•	Constructor
	•	Method:

void printInfo()



⸻

🔧 Exercise 2 – Create Methods to Organize Code

In WarehouseApp, instead of putting everything in main, create these methods:

1. Method to create packages

ArrayList<PackageItem> createPackages()

Do:
	•	Create an ArrayList
	•	Add 4–5 packages
	•	Return the list

⸻

2. Method to print all packages

void printAllPackages(ArrayList<PackageItem> packages)

Do:
	•	Use a for loop
	•	Call printInfo() for each package

⸻

⚖️ Exercise 3 – Method with If-Else

Create a method:

void checkWeight(PackageItem p)

Do:
	•	If weight > 10 → print "Heavy package"
	•	Else → print "Normal package"

⸻

🚀 Exercise 4 – Method for Priority Logic

Create:

void checkPriority(PackageItem p)

Do:
	•	If "HIGH" → "Process immediately"
	•	Else → "Standard processing"

⸻

🔁 Exercise 5 – Combine Everything

Create a method:

void processPackages(ArrayList<PackageItem> packages)

Do:
	•	Loop through packages
	•	For each package:
	•	Print info
	•	Call checkWeight(p)
	•	Call checkPriority(p)

⸻

🔢 Exercise 6 – Method that Returns a Value

Create:

int countHighPriority(ArrayList<PackageItem> packages)

Do:
	•	Loop through packages
	•	Count "HIGH" priority
	•	Return the count

⸻

🧠 Exercise 7 – Slightly Smarter Logic

Create:

void checkSpecialCase(PackageItem p)

Do:
	•	If weight > 10 AND "HIGH"
→ "Urgent heavy package"
	•	Else if "HIGH"
→ "Urgent"
	•	Else
→ "Normal flow"

⸻

🧩 Final Step – Clean main

Your main should look simple, like a control panel:

ArrayList<PackageItem> packages = createPackages();

printAllPackages(packages);
processPackages(packages);

int highCount = countHighPriority(packages);
System.out.println("High priority packages: " + highCount);


⸻

:jigsaw: Exercise – Shipping System


Step 1 – Create an Interface

Create an interface called Shippable.

Do:

Add a method:
double calculateShippingCost(double weight);



Step 2 – Create Two Classes

Create two classes that implement Shippable.



:truck: Class 1: 
StandardShipping

Rules:

Cost = weight * 1.0



:zap: Class 2: 
ExpressShipping

Rules:

Cost = weight * 2.5 + 5



:repeat: Step 3 – Use Them Together

Create a class ShippingApp with main.

Do:

• Create an ArrayList<Shippable>
• Add:


1 StandardShipping
1 ExpressShipping
(optionally more)



:gear: Step 4 – For Loop + Polymorphism

Do:

• Use a for loop
• For each object:


Call calculateShippingCost(10) (use weight = 10)
Print the result



:brain: Optional Small Challenge

• Print different messages depending on the cost:


If cost > 20 → "Expensive shipping"
Else → "Affordable shipping"

