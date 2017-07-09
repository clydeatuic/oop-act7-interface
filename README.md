# Activity: Interface

## Task 1

* Using Netbeans, create new java application.
* Create new project. (Project Name: 070717_Lastname_Interface)
* Create new package. (Package Name: Lastname_Task1)
* Create the following activity setup java codes (A, B, C, D and Task1Demo)
	```java
	//A.java
	public interface A {
	    void o();
	    void p();
	    void q();
	}
	```
	```java
	//B.java
	public interface B {
    	//no abstract methods yet...
	}
	```
	```java
	//C.java
	public interface C {
    	//no abstract methods yet...
	}
	```
	```java
	//D.java
	public class D implements A{
	    String d;
	    D(){
	        this.d = "No value";
	    }
	    D(String d){
	        this.d = d;
	    }
	    @Override
	    public void o(){
	        System.out.println("Class D implements method o");
	    }
	    public void p(){
	        System.out.println("Class D implements method p");
	    }
	    void q(){
	        System.out.println("Class D implements method q");
	    }
	}
	```
	```java
	//Task1Demo.java
	public class Task1Demo {
	    public static void main(String[] args) {
	        D d = new D();
	        System.out.println(d.getD());
	        d.o();
	        d.p();
	        d.q();
	    }
	}	
	```
* Debug the necessary java file in order to display the following output given
	![Task1](https://github.com/clydeatuic/oop-act7-interface/blob/master/task1.PNG)

## Task 2

* Using the same project, create new package. (Package Name: Lastname_Task2)
* Make sure to copy all the java codes from the previous package.
* Update B interface by adding the following requirements:
	> abstract methods r and s (these methods contains no paramater and doesn't return any value)
	> abstract method t that accepts a string parameter
	> abstract method u that accepts two string arguments and also return a string data type.
* Create new class E that implements A and B interfaces and follow the method implementation requirements specified below:
	Method | Method Body
	------------ | -------------
	o | Display a message "Class E implements method o
	p | Display a message "Class E implements method p
	q | Display a message "Class E implements method q
	r | Display a message "Class E implements method r
	s | Display a message "Class E implements method s
* Create a Task2Demo class that prints the following output.	
	![Task2](https://github.com/clydeatuic/oop-act7-interface/blob/master/task2.PNG)