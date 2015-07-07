# java-program
SELENIUM- TESTING -JAVA 
Part 1

1) What are instance and local variables? Give some examples.
Local variables are declared in methods, constructors, or blocks.
Local variables are created when the method, constructor or block is entered and the variable will be destroyed once it exits the method, constructor or block.
Instance variables are declared in a class, but outside a method, constructor or any block.
When a space is allocated for an object in the heap, a slot for each instance variable value is created.
3)What is the purpose of declaring a variable as final?
Any variable either member variable or local variable (declared inside method or block) modified by final keyword is called final variable. Final variables are often declare with static keyword in java and treated as constant. Here is an example of final variable in Java

public static final String LOAN = "loan";
LOAN = new String("loan") //invalid compilation error

Final variables are by default read-only.

4)What is an Abstract Class and what is it’s purpose? Provide some example
   Abstract class contains atlest one abstract method,.
abstract classVehicle
{
abstract void speed ();
void fast ()
{
system.out.println (“fast”)
}
}
public static void main
{
bike b=new bike();
b.speed ();
b.fast();
}
}
6)What is an abstract method? Provide some example
Define “abstract” keyword, 
abstract classVehicle
{
abstract void speed ();
void fast ()
{
system.out.println (“fast”)
}
}
public static void main
{
bike b=new bike();
b.speed ();
b.fast();
}
}
Part 2: Predict the output of following Java Programs.
Three marks questions (Totally 5 question: 5 X 3 = 15)
=========================================================
2)class Calculation{  
void sum(int a,int b){System.out.println(a+b);}  
 void sum(int a,int b,int c){System.out.println(a+b+c);}  
  public static void main(String args[]){  
Calculation obj=new Calculation();  
obj.sum(10,10,10);  
obj.sum(20,20);   }  }  
OUTPUT
30
40

3) class Bike{  
final int speedlimit=90;
void run(){  
 speedlimit=400;  
 }  
 public static void main(String args[]){  
 Bike obj=new  Bike();  
 obj.run();  
 }  
}
OUTPUT
90


4)
class A{  
void msg(){System.out.println("Hello");}  
}  
class B{  
void msg(){System.out.println("Welcome");}  
}  
class C extends A,B
   
Public Static void main(String args[]){  
   C obj=new C();  
   obj.msg
}  
}  
OUTPUT
Hello
Welcome
5)
abstract class Bank{    
abstract void getRateOfInterest();    
}    
class SBI extends Bank{    
void getRateOfInterest(){
System.out.println(“8”);
}    
}    
class PNB extends Bank{    
void getRateOfInterest(){
System.out.println(“7”);
}    
}    
class TestBank{    
public static void main(String args[]){    
Bank b=new SBI();    
b.getRateOfInterest();        
}
}
OUTPUT
8

Part 3: Write the program for following scenarios

Five marks questions (Totally 3 question: 3 X 5 = 15)




1)Write the program for student marks calculation using object and class.
////code/////
class Student2{
int rollno;
String name;
void insertRecord(int r,String n){
//method
rollno=r;
name=n;
}

void displayInformation(){System.out.println(rollno+" "+name);}//method
public static void main(String args[]){
Student2 s1=new Student2();
Student2 s2=new Student2();

 s1.insertRecord(111,"Karan");
s2.insertRecord(222,"Aryan");
s1.displayInformation();
s2.displayInformation();

}
}

       111 Karan
       222 Aryan
     


2)write the program for your choice using both class and interface (using inheritance concept)
	interface Parent
{
void show();
}

class Child implements Parent
{
public void show() 
{
System.out.println("Child");
}

public String toString()
{
System.out.println("toString");
}
}


///main() method
{
Parent p=new Child();
p.toString();
}

3)write the program for your choice using both class and interface (using inheritance concept)

class Animal{
void eat(){System.out.println("eating");}
}
class Dog extends Animal{
void eat(){System.out.println("eating fruits");}
}

class BabyDog extends Dog{
void eat(){System.out.println("drinking milk");}

public static void main(String args[]){
Animal a1,a2,a3;
a1=new Animal();
a2=new Dog();
a3=new BabyDog();

a1.eat();
a2.eat();
a3.eat();
}
} 
Output: eating
        eating fruits
        drinking Milk

	
