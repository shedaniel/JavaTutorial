# Beginners 1.1
We will put 1.1 into different sections
- Hello World
- Variables
- if / else if
- T[]
- While Loop
- For Loop
- For Loop in List
- Functions
- JOptionPane

### Hello World
A basic print is somewhat like this:
```java
System.out.println("Hello World");
```

### Variables
There are lots of types of variables:
- int
- long
- float
- double
- char
- boolean
- short

Or object typed:
- Byte
- Short
- Character
- Integer
- Long
- Float
- Double
- String

An example presented here:
```java
int a = 123;
long b;
String name = "Daniel";
```

### if / else / else if Statement
Conditions in Java (They create booleans):
- == (Equal)
- != (Not Equal)
- \> (Bigger)
- < (Smaller)
- \>= {Bigger or equal)
- <= (Smaller or equal)

Just simply put booleans inside _if_:
```java
boolean abc = true;
if (abc) {
	System.out.println("Hello");
}
```
Or condition inside:
```java
int a = 10;
int b = 12;
if (a < b) {
	System.out.println("Hello");
}
```
Use else to revert if statement:
```java
int a = 123;
int b = 1241;
if (a > b) {
	System.out.println("Hello");
}else {
	System.out.println("Bye");
}
```
Use ! to revert boolean:
```java
boolean abc = true;
if (!abc) {
	System.out.println("Hello");
}
```
And it also work in conditions:
```java
int a = 12314;
if (!(a < 21414)) {
	System.out.println("Hello");
}
```
You can also use these:
- && (and)
- || (or)

### T[]
T[] is like a list in python or pascal, you replace T with your type (such as String)
```java
String[] names = {"Daniel", "Ice Cream"};
```
The size of the list cannot be changed without making a new list.
You can modtify / get the list by this method:
```java
String[] names = {"Daniel", "Ice Cream"};
names[0] = "Chips";
System.out.println(names[1]);
```
The index of the first item in the list is 0. The first line set the item 0 to "Chips", and print out item 1 of names which is "Ice Cream".

To get the length of T[], simply to this:
```java
String[] names = {"Daniel", "Ice Cream"};
int length = names.length;
```

### While Loop
While loop is kinda kind to explain. The while statement continually executes a block of statements while a particular condition is true. Its syntax can be expressed as:
```java
while (expression) {
     statement(s)
}
```
The while statement evaluates expression, which must return a boolean value. If the expression evaluates to true, the while statement executes the statement(s) in the while block. The while statement continues testing the expression and executing its block until the expression evaluates to false. Using the while statement to print the values from 1 through 10 can be accomplished as in the following code:
```java
int count = 1;
while (count < 11) {
	System.out.println("Count is: " + count);
	count++;
}
```

### For Loop
The for statement provides a compact way to iterate over a range of values. Programmers often refer to it as the "for loop" because of the way in which it repeatedly loops until a particular condition is satisfied. The general form of the for statement can be expressed as follows:
```java
for (initialization; termination; increment) {
	statement(s)
}
```
You can make a basic counter like so:
```java
for (int i = 0; i < 10; i++) {
	System.out.println(i);
}
```
This code will output:
```
0
1
2
3
4
5
6
7
8
9
```
### For Loop in List
The for statement also has another form designed for iteration through Collections and arrays This form is sometimes referred to as the enhanced for statement, and can be used to make your loops more compact and easy to read.
```java
int[] numbers = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
for (int i : numbers) {
	System.out.println(i);
}
```
This code will loop over each item in the list numbers.
### Functions
Functions in java are known as void, a basic function looks like this:
```java
public class Main {
	public static void testFunction() {
    	//Random Stuff
    }
}
```
testFunction is a method we defined in class Main. Notice a few things about foo.
- _static_ means this method belongs to the class Main and not to a specific instance of Main. Which means we can call the method from a different class like that Main.testFunction().
- _void_ means this method doesn't return a value. Methods can return a single value in Java and it has to be defined in the method declaration. However, you can use return by itself to exit the method.
This method doesn't get any arguments, but of course Java methods can get arguments as we'll see further on.
##### Arguments
You can add arguments to an function:
```java
public static void randomStuff(int a, int b) {
	int sum = a + b;
    System.out.println(sum);
}
```
This function will require two variables to execute, and basically this just add the two and print them.
### JOptionPane
Option Pane is a easy way to display information to the user. A very basic code is like this:
```java
JOptionPane.showMessageDialog(null, "Some random text...");
```
Of course you can add custom titles with custom icons:
```java
JOptionPane.showMessageDialog(null, "Hello World", "Random Title", messageType);
```
There are these following message types:
- ERROR_MESSAGE
- INFORMATION_MESSAGE
- WARNING_MESSAGE
- QUESTION_MESSAGE
- PLAIN_MESSAGE
A simple usage here:
```java
JOptionPane.showMessageDialog(null, "You are banned from Milk!", "Error", JOptionPane.ERROR_MESSAGE);
```