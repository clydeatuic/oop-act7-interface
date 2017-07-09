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
	![Task1.5](https://octodex.github.com/images/yaktocat.png)