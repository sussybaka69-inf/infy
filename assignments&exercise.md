![Capture](https://user-images.githubusercontent.com/105406807/168093235-4c677dcb-a59c-4c15-8431-c2c5f4c9dc93.PNG)
```java
class Tester {
	public static void main(String[] args) {
		// Implement your code here 
				int rate=7,time=3,p=3250;
		System.out.println((float)(p*rate*time)/100);
	}
}


```

![Capture](https://user-images.githubusercontent.com/105406807/168097613-1b1ad2bf-4027-4c0f-8ea7-c62155d20621.PNG)
```java
class Tester {
	public static void main(String[] args) {
		// Implement your code here 
		float pi=3.14f;
		int radius=10;	
		System.out.println( pi*radius*radius);
		
	}
}


```
![Capture](https://user-images.githubusercontent.com/105406807/168098599-7c5b1dc1-8dd3-4290-b5b5-fa8c6795f506.PNG)
```java
class Tester {
	public static void main(String[] args) {
		// Implement your code here 
				float f=50f;
		System.out.println(((f-32)/9)*5 );
	}
}
```
![Capture](https://user-images.githubusercontent.com/105406807/168419068-e8fff37d-949e-469c-8478-faa9470f6173.PNG)
```java
class Tester {
	public static void main(String[] args) {
		// Implement your code here 
		int num1=3,num2=4,num3=1;
if(num1>num2) {
	if(num1>num3) {
		System.out.println(num1);
	}
	else {
		System.out.println(num3);
	}
}
else {
	if(num2>num3) {
		System.out.println(num2);
	}
	else {
		System.out.println(num3);
	}
}

	}
}


```
# Luck Number
```java
public class Tester {
	private static int num;
	int g;
	public static void main(String[] args) {
		int x=15,temp=0,rev=0,k=0;
		String s=""+x;
		for(int i=0;i<s.length();i++) {
			if(i%2!=0) {
				k+=Math.pow(Character.getNumericValue(s.charAt(i)),2) ;
			}
			
			
		}
		if(k%9==0) {
			System.out.println("the number "+x+" is a lucky number");
		}
		else {
			System.out.println("the number "+x+" is  not a lucky number");
		}
	}
}


```
# LCM
```java
public class Tester {
	private static int num;
	int g;
	public static void main(String[] args) {
		int x=7,y=9,lcm;
		lcm=(x>y)?x:y;
			while(true) {
				if(lcm%x==0&&lcm%y==0) {
					System.out.println("lcm is "+lcm);
					break;
				}
				lcm++;
		}
	}
}
```
# CHICKEN AND RABBIT
```java
public class Tester {
	public static void main(String[]args) {
	int heads=150,legs=500;
	int r=0,c=0;
	if((heads>legs)||(heads==0)||(legs%2!=0))
	{
	System.out.println("Thenumberofchickensandrabbitscannotbefound");
	}
	else{
	r=((legs-(2*heads))/2);
	c=(heads-r);
	System.out.println("Chickens="+c);
	System.out.println("Rabbits="+r);
	}
	}
}
```
# MAX NO OF CHAR
```JAVA
class Tester {

	public static int findHighestOccurrence(String str){
		//Implement your code here and change the return value accordingly
			
		int c=0,cmax=1;
		for(int i=0;i<str.length();i++) {
			for(int j=0;j<str.length();j++) {
				if(str.charAt(i)==str.charAt(j)) {
					c++;
				
					
					}
				
				if(c>cmax) {
					cmax=c;
				
				}
				
			
			}
			c=0;
		}
      return cmax;
	
	}
  
	
	public static void main(String args[]){
	    String str = "success";
	    System.out.println(findHighestOccurrence(str));
	}
}
```
# STORING OBJECTS IN A ARRAY
```java
class Teacher {
    //Implement your code here
	private String teacherNameString;
	private String subjectString;
	private double salary;
	public Teacher(String teacherNameString, String subjectString, double salary) {
		this.teacherNameString = teacherNameString;
		this.subjectString = subjectString;
		this.salary = salary;
	}
	public String getTeacherNameString() {
		return teacherNameString;
	}
	public void setTeacherNameString(String teacherNameString) {
		this.teacherNameString = teacherNameString;
	}
	public String getSubjectString() {
		return subjectString;
	}
	public void setSubjectString(String subjectString) {
		this.subjectString = subjectString;
	}
	public double getSalary() {
		return salary;
	}
	public void setSalary(double salary) {
		this.salary = salary;
	}
	
}


class Tester {
	public static void main(String[] args) {
	    // Implement your code here 
		Teacher t1=new Teacher("Alex","JAva",1200l);
		Teacher t2=new Teacher("Jhon","rdbms",800l);
		Teacher t3=new Teacher("Sam","Networking",900l);
		Teacher t4=new Teacher("Maria","Python",900l);
		Teacher []teacherArr= {t1,t2,t3,t4};
		for(Teacher t:teacherArr) {
			System.out.println("Name :"+t.getTeacherNameString()+", Subject:"+t.getSubjectString()+", Salary:"+t.getSalary());
		}
	}
}
```
![Capture](https://user-images.githubusercontent.com/105406807/168269630-b9ec96db-f007-4330-81e2-ce7e3d52780b.PNG)
```java
class Tester{

    public static String removeWhiteSpaces(String str){
 	    	String d="";
	        for(int i=0;i<str.length();i++){
	            if(str.charAt(i)!=' ') {
	            	d+=str.charAt(i);
	            }
	        }
	        return d;
    }
	
	public static void main(String args[]){
		String str = "Hello   How are you   ";
		str = removeWhiteSpaces(str);
		System.out.println(str);
	}
}
```
![Capture](https://user-images.githubusercontent.com/105406807/168270880-1e51ccbe-133e-4674-85f9-873ec5a78ad6.PNG)
```java
class Tester {
    
    public static int calculateSumOfEvenNumbers(int[] numbers){
        //Implement your code here and change the return value accordingly
        	int d=0;
	    	for(int i:numbers) {
	    		if(i%2==0) {
	    			d+=i;
	    			
	    		}
	    	}
	        return d;
	    }
    
	public static void main(String[] args) {
		int[] numbers = {68,79,86,99,23,2,41,100};
		System.out.println("Sum of even numbers: " +calculateSumOfEvenNumbers(numbers));
	}
}
```

![Capture](https://user-images.githubusercontent.com/105406807/168306248-c46fc0e7-c56a-46a8-a42d-5e5717d57b70.PNG)
```java
class Calculator {

	// Implement your code here
	public double findAverage(int number1,int number2,int number3){
	    double x=(number1+number2+number3)/(double)3;
	    return (Math.round(x*100.0)/100.0);
	}
}

class Tester {

	public static void main(String args[]) {
		Calculator calculator = new Calculator();
		// Invoke the method findAverage of the Calculator class and display the average
		Calculator.findAverage(number1,number3,number2);
	}
}

```
![Capture](https://user-images.githubusercontent.com/105406807/168430017-c9563213-37b4-4b35-a87c-dcf1e12ec70b.PNG)

```java
class Tester{
    
    public static String moveSpecialCharacters(String str){
		//Implement your code here and change the return value accordingly
  		String alpha="";
			String sy="";
			for(int i=0;i<str.length();i++){
			        if (Character.isAlphabetic(str.charAt(i))) {
			            alpha+=str.charAt(i);
			        }
			        else{
			            		            sy+=str.charAt(i);

			        }
			            

			}
	        return alpha+=sy;
    }
	
	public static void main(String args[]){
	    String str = "He@#$llo!*&";
	    System.out.println(moveSpecialCharacters(str));
	}
	
}
```
#TO GET SUM OF ALL ENTERED NUMBERS
```JAVA
class Tester {
	public static void main(String[] args) {
		int inputNumber = 7865;
		int sumOfDigits = 0;
		int temp = 0;

		while (inputNumber > 0) {
			temp = inputNumber % 10;
			sumOfDigits += temp;
			inputNumber = inputNumber / 10;
		}

		System.out.println("Sum of digits are : " + sumOfDigits);
	}
}


########################################ARNOLDS NUMBER
	int x=1635,temp=0,rev=0;
		String s=""+x;
		while(x>0) {
			
			temp=x%10;
			rev+=Math.pow(temp, s.length());
			x=x/10;
		}
	System.out.println(rev);
````
![Capture](https://user-images.githubusercontent.com/105406807/168430076-cf556511-c17a-4e6d-bc12-ebd9d25d83ff.PNG)



```java
class Tester {
	public static void main(String[] args) {
		int a=1,b=4,c=6,d;
		d=b*b-4*a*c;
		if(d>0) {
			System.out.println(((-b-d)/2*a)+"");
			System.out.println(((-b+d)/2*a)+"");
			

		}
		else if(d<0){
			
			System.out.println("The equation has no real root");
		}
		else {
			System.out.println((-b-d)/2*a);	

	}
	}
}
```
![Capture](https://user-images.githubusercontent.com/105406807/168430638-7705b86b-7932-414b-b104-27dc64100553.PNG)
```java
class Tester {
	public static void main(String[] args) {
	int q=2,d=10,fb;
		char food='V';
		if (food=='N') {
			fb=q*15;
		}
		else {
			fb=q*12;

		}
		if (d>3&&d<6) {
			fb+=d;
		}
		else if(d>6) {
			
			fb+=((d-6)*2)+3;
			

		}
System.out.println(fb);
	}
}


```
![Capture](https://user-images.githubusercontent.com/105406807/168436483-26b9638b-06a0-4900-a5ff-7ddf30040aab.PNG)
```java
class Tester {
	public static void main(String[] args) {
	int acc_no=1001,sal=40000,accb=250000,c=0,cb=0,count=0,loanexp=300000,emiexp=30;
	String lt="Car";
	while(acc_no>0) {
		acc_no=acc_no/10;
		count++;
		if(acc_no==1) {
			cb=1;
		}
		
	}
	if(count==4) {
		c=1;
	}
	if(c==1&&cb==1) {
		switch (lt) {
		case "Car":
			if(loanexp<=500000&&emiexp<=36) {
				System.out.println("eligible loan amount= "+500000+"\nnumber of EMIs="+36);
				break;
			}
			else {
				System.out.println("no can do");
				break;
			}
			
		case "House":
			if(loanexp<=6000000&&emiexp<=60) {
				System.out.println("eligible loan amount= "+6000000+"\nnumber of EMIs="+60);
				break;
			}
			else {
				System.out.println("no can do");
				break;
			}
		case "Business":
			if(loanexp<=7500000&&emiexp<=84) {
				System.out.println("eligible loan amount= "+7500000+"\nnumber of EMIs="+84);
				break;
			}
			else {
				System.out.println("no can do");
				break;

			}
				
			
			
		}
	
	}
	else {
		System.out.println("validation failed");

	}
	
	}
	}
```

![Capture](https://user-images.githubusercontent.com/105406807/168442733-d7185425-5460-492f-9f5c-812e5cbd80cb.PNG)
```java
package tt;
class gf {
	    
	    public static void main(String args[]){
	  int d=31,m=7,y=11;
	  y+=2000;
	  if(d==31) {
		  if(m==12) {
			  y+=1;
			  m=1;
			  d=1;
		  }
		  else {
			  m+=1;
			  d=1;
		  }
	  }
	  else {
		  d+=1;
	  }
	   
	  System.out.println(d+"-"+m+"-"+y);
	    
	    }
	  }
	    
```
![Capture](https://user-images.githubusercontent.com/105406807/168442922-f95712dd-9ee8-4f18-ae57-efd5ca302c63.PNG)
```java
class Tester {
	public static void main(String[] args) {
	    	int i=6;
	    	if(i%3==0||i%5==0) {
	    		if(i%3==0&&i%5==0) {
	    			System.out.println("zoom");
	    		}
	    		else if(i%3==0){
	    			System.out.println("zip");    			
	    		}
	    		else {
	    			System.out.println("zap");    			

	    		}
	    	}
	    	else {
    			System.out.println("invalid");    			

	    	}
	    	
	    	
	    	}
	    
	    
}
```
![Capture](https://user-images.githubusercontent.com/105406807/168443313-79be6adc-42fe-4438-ac23-1c32decb18e1.PNG)
```java
class Tester {
	public static void main(String[] args) {
    	int i=46763,g=i,rev=0,t;
	    	while(g>0) {
	    		t=g%10;
	    		rev=rev*10+t;
	    		g=g/10;
	    		
	    		
	    	}
	    	if(i==rev) {
	    	System.out.println(i+" is a Palindrome");
	    	}
	    	else {
		    	System.out.println(i+"is not a Palindrome");

	    	}
	    	
	    		
	    
	    	
	    	}
	    
	    
}

```
![Capture](https://user-images.githubusercontent.com/105406807/168443980-c553d2f2-e376-4a47-b9aa-71600fceae83.PNG)
```java
class Tester {
	public static void main(String[] args) {
	    	int i=45,g=i,t,y=1000;
	    	int x=i;	
	    	while(g>0) {
	    		t=g%10;
	    		i*=t;
	    		g=g/10;
	    		    		
	    	}
	    	
	    if(i==y) {
	    	System.out.println(x+" is a seed of "+y);

	    }
	    else {
	    	System.out.println(x+" is not a seed of "+y);

	    }
	    		
	    
	    	
	    	}
	    
}
```
<img width="739" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168465269-581e2f76-ef7b-495f-8778-14fbcaecb1ef.PNG">

```java
class Calculator {
public int num;
public int sumOfDigits( ){
    int sum=0;
    int temp;
    while(num>0){
        temp=num%10;
        sum+=temp;
        num=num/10;
    }
    return sum;
}
	// Implement your code here

}

class Tester {

	public static void main(String args[]) {

		Calculator calculator = new Calculator();
		calculator.num=123;
		// Assign a value to the member variable num of Calculator class
       System.out.println(calculator.sumOfDigits());
		// Invoke the method sumOfDigits of Calculator class and display the output

	}
}
```
<img width="925" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168628489-c2e6ec2d-1088-4f4a-84db-77248b3d9ef6.PNG">

```java

class Employee{
private String employeeId;
private String employeeName;
private int salary;
private int bonus;
private int jobLevel;
public String getEmployeeId(){
return employeeId;
}
public void setEmployeeId(String employeeId){
this.employeeId=employeeId;
}
public String getEmployeeName(){
return employeeName;
}
public void setEmployeeName(String employeeName){
this.employeeName=employeeName;
}
public int getSalary(){
return salary;
}
public void setSalary(int salary){
this.salary=salary;
}
public int getBonus(){
return bonus;
}
public void setBonus(int bonus){
this.bonus=bonus;
}
public int getJobLevel(){
return jobLevel;
}
public void setJobLevel(int jobLevel){
this.jobLevel=jobLevel;
}
public void calculateSalary() {
		if (this.jobLevel >= 4) {
			this.bonus = 100;
		} else {
			this.bonus = 50;
		}
		this.salary += this.bonus;
	}
}
class Tester {

	public static void main(String args[]) {
Employee employee=new Employee();
employee.setEmployeeId("C101");
employee.setEmployeeName("Steve");
employee.setSalary(650);
employee.setJobLevel(4);
employee.calculateSalary();
System.out.println("Employee Details");
		System.out.println("Employee Id: " +employee.getEmployeeId());
		System.out.println("Employee Name: " + employee.getEmployeeName());
		System.out.println("Salary: " + employee.getSalary());

	}
}
```
<img width="624" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168650596-e5d4eb5a-19dd-4a9f-b418-062ead707fb5.PNG">

```java
class Bill{
    //Implement your code here
    private static int counter;
    private String billId;
    private String paymentMode;
    
    static{
        counter=9000;
    }
    
    public Bill(String paymentMode){
        this.paymentMode=paymentMode;
        billId="B"+ ++counter;
    }
    
    public void setBillId( String billId){
        this.billId=billId;
    }
    public String getBillId(){
        return billId;
    }
    public void setPaymentMode( String paymentMode){
        this.paymentMode=paymentMode;
    }
    public String getPaymentMode(){
        return paymentMode;
    }
    public static int getCounter(){
        return counter;
    }
}

class Tester {
    public static void main(String[] args) {

        Bill bill1 = new Bill("DebitCard");
        Bill bill2 = new Bill("PayPal");
        
        //Create more objects and add them to the bills array for testing your code
              
        Bill[] bills = { bill1, bill2 };
              
        for (Bill bill : bills) {
            System.out.println("Bill Details");
            System.out.println("Bill Id: " + bill.getBillId());
            System.out.println("Payment method: " + bill.getPaymentMode());
            System.out.println();
       }
    }
}
```
<img width="321" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168782205-02ea7ce4-8696-44d8-a134-bbf42cb94bed.PNG">

```java
class CabServiceProvider{
    //Implement your code here
    private String cabServiceName;
private int totalCabs;

public CabServiceProvider(String cabServiceName, int totalCabs) {
	this.cabServiceName = cabServiceName;
	this.totalCabs = totalCabs;
}

public String getCabServiceName() {
	return cabServiceName;
}

public void setCabServiceName(String cabServiceName) {
	this.cabServiceName = cabServiceName;
}

public int getTotalCabs() {
	return totalCabs;
}

public void setTotalCabs(int totalCabs) {
	this.totalCabs = totalCabs;
}
public double calculateRewardPrice(Driver driver){
	double b=0;
	float f=driver.getAverageRating();
	switch(cabServiceName) {
	case "Halo":
		if(f>=4&&f<4.5) {
			b= 5*f;
			break;
		}
		else if(f>=4.5&&f<=5) {
			b= 10*f;
			break;
		}
		else {
			b=0;
		}
	case "Aber":
		if(f>=4&&f<4.5) {
			b= 3*f;
			break;
		}
		else if(f>=4.5&&f<=5) {
			b= 8*f;
			break;
		}
		else {
			b=0;
		}
		
	}
 return (Math.round(b*100.0)/100.0);	
}
}

class Driver {
	
	private String driverName;
	private float averageRating;
	
	public Driver(String driverName, float averageRating){
		this.driverName=driverName;
		this.averageRating=averageRating;
	}
	
	public String getDriverName(){
		return this.driverName;
	}
	
	public void setDriverName(String driverName){
		this.driverName=driverName;
	}
	
	public float getAverageRating(){
		return this.averageRating;
	}
	
	public void setAverageRating(float averageRating){
		this.averageRating=averageRating;
	}

    //DO NOT MODIFY THE METHOD
    //Your exercise might not be verified if the below method is modified
    public String toString(){
        return "Driver\ndriverName: "+this.driverName+"\naverageRating: "+this.averageRating;
    }
}

class Tester {
	
	public static void main(String args[]){
	    CabServiceProvider cabServiceProvider1 = new CabServiceProvider("Halo", 50);

		Driver driver1 = new Driver("Luke", 4.8f);
		Driver driver2 = new Driver("Mark", 4.2f);
		Driver driver3 = new Driver("David", 3.9f);
		
		Driver[] driversList = { driver1, driver2, driver3 };
		for (Driver driver : driversList) {
			System.out.println("Driver Name: "+driver.getDriverName());
			double bonus = cabServiceProvider1.calculateRewardPrice(driver);
			if (bonus>0)
				System.out.println("Bonus: $"+bonus+"\n");
			else
				System.out.println("Sorry, bonus is not available!");
		}
		
		//Create more objects of CabServiceProvider and Driver classes for testing your code
	}
}


```
Aggregation - Assignment 3
25m 37s
Problem Statement
Jasmine 
Girls Hostel wants you to create a small application for them to assign rooms to members. You need to implement the classes based on the class diagram and description given below.


<img width="282" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168803921-8a8bab0f-cac5-4135-a282-0b18301e3d56.PNG">


Member

Member(int memberId, String name)

Initialize the memberId and name instance variables appropriately with the values passed to the constructor.
Implement the appropriate getter and setter methods.

 

Room

Room()

Generate the roomNo using the static variable roomCounter. The value of roomNo should start from 500 and should be incremented by 1 for the subsequent values. Initialize the roomNoCounter in static block.

Initialize the capacity instance variable to 4.

Implement the appropriate getter and setter methods. 

 

Admin 

assignRoom(Room[] rooms, Member member)

Assign a room to the member using the below conditions:

One room can accommodate 4 members. 

Allocate the first room that is empty.

Once a room is fully occupied, only then a new room should be assigned.

Update the capacity of the allocated room accordingly.

Test the functionalities using the provided Tester class.

 

Sample Input and Output

Input

<img width="228" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168803791-5895f755-3649-4594-bf07-0cce22276a77.PNG">










Note: room1, room2, room3 , room4 and room5 are objects of Room class.

Output



Download the Java project from here to solve this assignment in Eclipse.

```java
class Room {
    //Implement your code here 
private int roomNo;
private  int capacity;
private static int roomCounter;

static {
	roomCounter=500;
}

public Room() {
	this.roomNo=roomCounter++;
	capacity=4;
}
public int getRoomNo() {
	return roomNo;
}
public void setRoomNo(int roomNo) {
	this.roomNo = roomNo;
}
public  int getCapacity() {
	return capacity;
}
public  void setCapacity(int capacity) {
	this.capacity = capacity;
}
public static int getRoomCounter() {
	return roomCounter;
}
public static void setRoomCounter(int roomCounter) {
	Room.roomCounter = roomCounter;
}
    //Uncomment the below method after implementation before verifying 
    //DO NOT MODIFY THE METHOD
  
    public String toString(){
        return "Room\nroomNo: "+this.roomNo+"\ncapacity: "+this.capacity;
    }
  
}

class Member {
	//Implement your code here 
	private int memberId;
private String name;
private Room room;
public Member(int memberId, String name) {
	this.memberId = memberId;
	this.name = name;
}
public int getMemberId() {
	return memberId;
}
public void setMemberId(int memberId) {
	this.memberId = memberId;
}
public String getName() {
	return name;
}
public void setName(String name) {
	this.name = name;
}
public Room getRoom() {
	return room;
}
public void setRoom(Room room) {
	this.room = room;
}

	
	//Uncomment the below method after implementation before verifying 
    //DO NOT MODIFY THE METHOD
  
    public String toString(){
        return "Member\nmemberId: "+this.memberId+"\nname: "+this.name;
    }
 
}

class Admin {
	//Implement your code here 
public void  assignRoom(Room[] rooms, Member member) {

		for(Room i:rooms) {
			if(i.getCapacity()>0) {
				member.setRoom(i);
				i.setCapacity(i.getCapacity()-1);
				break;
			}
			
		}
	}
}


class Tester {
	public static void main(String args[]) {
		Room room1 = new Room();
		Room room2 = new Room();
		Room room3 = new Room();
		Room room4 = new Room();
		Room room5 = new Room();

		Room[] totalRooms = { room1, room2, room3, room4, room5 };

		Admin admin = new Admin();

		Member member1 = new Member(101, "Serena");
		Member member2 = new Member(102, "Martha");
		Member member3 = new Member(103, "Nia");
		Member member4 = new Member(104, "Maria");
		Member member5 = new Member(105, "Eva");
		
		Member[] members = { member1, member2, member3, member4, member5 };
		
		for (Member member : members) {
			admin.assignRoom(totalRooms, member);
			if(member.getRoom()!=null) {
				System.out.println("Hi "+member.getName()+"! Your room number is "+member.getRoom().getRoomNo());
			}
			else {
				System.out.println("Hi "+member.getName()+"! No room available");
			}
		}
	}
} 
 



```
Method Overloading - Exercise 1
22m 8s
Problem Statement
The Point class is used for representing a point with two coordinates.

Implement the class Point based on the class diagram and description given below.
<img width="164" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168874429-a2cf1268-afa9-4f95-af8b-075db086aade.PNG">



 

Method Description

Point(double xCoordinate , double yCoordinate )

Initialize the instance variables xCoordinate and yCoordinate appropriately with the values passed to the constructor.
calculateDistance()

Calculate and return the distance of the point from the origin (0,0). The distance can be calculated using the formula given below. The distance should be rounded off to 2 decimal digits.
     distance=√((x2-x1)2+(y2-y1)2), where x1 and x2 are values of x-coordinates of two points and y1 and y2 are values of y-coordinates of two points

calculateDistance(Point point)

Calculate and return the distance of the point from the 'point' passed to the method. The distance should be rounded off to 2 decimal digits.
Hints

Use Math.sqrt(double d) method to calculate the square root

Use Math.round(double d) method to round off the values

Implement the getter and setter methods appropriately.

 

Test the functionali<img width="312" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168874522-fa93beca-6d63-4986-831e-262aad8dcbea.PNG">
ties using the provided Tester class. 
```java
class Point {
    //Implement your code here
    private  double xCoordinate;
private  double yCoordinate;

public Point(double xCoordinate, double yCoordinate) {
	super();
	this.xCoordinate = xCoordinate;
	this.yCoordinate = yCoordinate;
	
	
}

public double getxCoordinate() {
	return xCoordinate;
}

public void setxCoordinate(double xCoordinate) {
	this.xCoordinate = xCoordinate;
}

public double getyCoordinate() {
	return yCoordinate;
}

public void setyCoordinate(double yCoordinate) {
	this.yCoordinate = yCoordinate;
}
public double calculateDistance() {
	double x2=xCoordinate,x1=0.0,y2=yCoordinate,y1=0;
	double distance=Math.sqrt((x2-x1)*(x2-x1)+(y2-y1)*(y2-y1));
	return Math.round(distance*100.0)/100.0;
}
public double calculateDistance(Point point) {
	double x2=xCoordinate,x1=point.xCoordinate,y2=yCoordinate,y1=point.yCoordinate;
	double distance=Math.sqrt((x2-x1)*(x2-x1)+(y2-y1)*(y2-y1));
	return Math.round(distance*100.0)/100.0;
	
}
}


class Tester {

	public static void main(String[] args) {
		Point point1 = new Point(3.5, 1.5);
        Point point2 = new Point(6, 4);
                                
        System.out.println("Distance of point1 from origin is "+point1.calculateDistance());
        System.out.println("Distance of point2 from origin is "+point2.calculateDistance());
        System.out.println("Distance of point1 from point2 is "+point1.calculateDistance(point2));
        
        //Create more objects for testing your code                

	}
}



```
<img width="549" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168886626-8bfeefac-886e-4221-ad9c-9ed95a78de69.PNG">
<img width="245" alt="Capture" src="https://user-images.githubusercontent.com/105406807/168886702-073e677d-0a4c-4931-ace5-1b7166120f36.PNG">

```java
class Bill{
    //Implement your code here
	public double findPrice(int itemId) {
		switch(itemId) {
		case 1001:
			return 25;
		case 1002:
			return 20;
		case 1003:
			return 23;
		case 1004:
			return 18;
		default:
			return 0;
		}
	
	}
	public double findPrice(String brandName,String itemType,int size) {
		double b=0;
		switch(brandName) {
		case "Puma":
			switch(itemType) {
			case "T-shirt":
				if(size==34||size==36) {
					b=25;
					
				}
				else {
					b=0;
					
				}
				break;
			case"Skirt"	:
				if(size==38||size==40) {
					b=20;
					
				}
				else {
					b=0;
					
				}
				break;
				
			}
			break;
		case "Reebok":
			switch(itemType) {
			case "T-shirt":
				if(size==34||size==36) {
					b=23;
					
				}
				else {
					b=0;
					
				}
				break;
			case"Skirt"	:
				if(size==38||size==40) {
					b=18;
					
				}
				else {
					b=0;
					
				}
				break;
			
			
		}
		
}
		return b;
}
}



```
<img width="703" alt="Capture" src="https://user-images.githubusercontent.com/105406807/169072918-26e7ba29-6a5c-4fc6-9249-60c8008b2406.PNG">
<img width="688" alt="Capture" src="https://user-images.githubusercontent.com/105406807/169073056-bce47409-f199-453b-a68d-28ffed764b4b.PNG">
<img width="659" alt="Capture" src="https://user-images.githubusercontent.com/105406807/169073210-86709fd9-f8ee-4d85-bec8-fc050b9eb136.PNG">


```java
class Employee {
      
    //Implement your code here 
    private int employeeId;
private String employeeName;
private double salary;
public Employee(int employeeId, String employeeName) {
	super();
	this.employeeId = employeeId;
	this.employeeName = employeeName;
}
public int getEmployeeId() {
	return employeeId;
}
public void setEmployeeId(int employeeId) {
	this.employeeId = employeeId;
}
public String getEmployeeName() {
	return employeeName;
}
public void setEmployeeName(String employeeName) {
	this.employeeName = employeeName;
}
public double getSalary() {
	return salary;
}
public void setSalary(double salary) {
	this.salary = salary;
}

    //Uncomment the below method after implementation before verifying 
    //DO NOT MODIFY THE METHOD
    
    public String toString(){
        return "Employee\nemployeeId: "+this.getEmployeeId()+"\nemployeeName: "+this.getEmployeeName()+"\nsalary: "+this.getSalary();
    }
    
}


class PermanentEmployee extends Employee {
      
    //Implement your code here 
    	private double basicPay;
	private double hra;
	private float experience;
	public PermanentEmployee(int empId,String name,double basicPay, double hra, float experience) {
		super(empId,name);
		this.basicPay = basicPay;
		this.hra = hra;
		this.experience = experience;
		
	}
	public double getBasicPay() {
		return basicPay;
	}
	public void setBasicPay(double basicPay) {
		this.basicPay = basicPay;
	}
	public double getHra() {
		return hra;
	}
	public void setHra(double hra) {
		this.hra = hra;
	}
	public float getExperience() {
		return experience;
	}
	public void setExperience(float experience) {
		this.experience = experience;
	}

	public void calculateMonthlySalary(){
		int vc=0;
		if(experience<3) {
			vc=0;
		}
		else if(experience>=3&&experience<5) {
			vc=5;
		}
		else if(experience>=5&&experience<10) {
			vc=7;
		}
		else if(experience>=10) {
			vc=12;
		}
		
		double s=basicPay+hra+basicPay*((float)vc/100);
		setSalary(s);
	}
    
    //Uncomment the below method after implementation before verifying 
    //DO NOT MODIFY THE METHOD
    
    public String toString(){
        return "PermanentEmployee\nemployeeId: "+this.getEmployeeId()+"\nemployeeName: "+this.getEmployeeName()+"\nsalary: "+this.getSalary()+"\nbasicPay: "+this.getBasicPay()+"\nhra: "+this.getHra()+"\nexperience: "+this.getExperience();
    }
    
}

class ContractEmployee extends Employee {
     
    //Implement your code here 
    private double wage;
private float hoursWorked;
public ContractEmployee(int empId,String name,double wage, float hoursWorked) {
	super(empId,name);
	this.wage = wage;
	this.hoursWorked = hoursWorked;
}
public double getWage() {
	return wage;
}
public void setWage(double wage) {
	this.wage = wage;
}
public float getHoursWorked() {
	return hoursWorked;
}
public void setHoursWorked(float hoursWorked) {
	this.hoursWorked = hoursWorked;
}

public void calculateSalary() {
	setSalary(this.hoursWorked*this.wage);
}
    
    //Uncomment the below method after implementation before verifying 
    //DO NOT MODIFY THE METHOD
    
    public String toString(){
        return "ContractEmployee\nemployeeId: "+this.getEmployeeId()+"\nemployeeName: "+this.getEmployeeName()+"\nsalary: "+this.getSalary()+"\nwage: "+this.getWage()+"\nhoursWorked: "+this.getHoursWorked();
    }
    
}

class Tester {
      
    public static void main(String[] args) {
      
        PermanentEmployee permanentEmployee = new PermanentEmployee(711211, "Rafael", 1855, 115, 3.5f);
	    permanentEmployee.calculateMonthlySalary();
	    System.out.println("Hi "+permanentEmployee.getEmployeeName()+", your salary is $"+permanentEmployee.getSalary());
	            
	    ContractEmployee contractEmployee = new ContractEmployee(102, "Jennifer", 16, 90);
	    contractEmployee.calculateSalary();
	    System.out.println("Hi "+contractEmployee.getEmployeeName()+", your salary is $"+contractEmployee.getSalary());
	        
	    //Create more objects for testing your code
    }
      
}
```
```java
class User{
    //Implement your code here
    private int id;
private String userName;
private String emailId;
private double walletBalance;
public User(int id, String userName, String emailId, double walletBalance) {
	this.id = id;
	this.userName = userName;
	this.emailId = emailId;
	this.walletBalance = walletBalance;
}
public int getId() {
	return id;
}
public void setId(int id) {
	this.id = id;
}
public String getUserName() {
	return userName;
}
public void setUserName(String userName) {
	this.userName = userName;
}
public String getEmailId() {
	return emailId;
}
public void setEmailId(String emailId) {
	this.emailId = emailId;
}
public double getWalletBalance() {
	
		return walletBalance;	
	
	
}
public void setWalletBalance(double walletBalance) {
	this.walletBalance = walletBalance;
}
public boolean makePayment(double billAmount) {
	
	if(getWalletBalance()-billAmount>=0){
	    this.setWalletBalance(getWalletBalance()-billAmount);
		return true;		
	}
	else {
		return false;
	}
	
}
}

class PremiumUser extends User {
    //Implement your code here
    	private int rewardPoints;
	
	
	public PremiumUser(int id, String userName, String emailId, double walletBalance) {
		super( id,  userName,  emailId,  walletBalance);
		
	}


	public int getRewardPoints() {
		return rewardPoints;
	}


	public void setRewardPoints(int rewardPoints) {
		this.rewardPoints = rewardPoints;
	}
@Override
	public boolean makePayment(double billAmount) {
		if(getWalletBalance()-billAmount>=0) {
			setRewardPoints((int)(getRewardPoints()+(billAmount/10)));
			this.setWalletBalance(getWalletBalance()-billAmount);

			return true;
			
			
		}
		else {
			return false;
			
		}
		
		
	}
}

class Tester {

    public static void main(String[] args) {

        User user = new User(101, "Joe", "joe@abc.com", 100);

		PremiumUser premiumUser = new PremiumUser(201, "Jill", "jill@abc.com", 300);

		processPayment(user, 70);

		processPayment(premiumUser, 150);

		processPayment(premiumUser, 80);

		processPayment(premiumUser, 120);

    }

    public static void processPayment(User user, double billAmount) {
        if (user.makePayment(billAmount)) {
			System.out.println("Congratulations " + user.getUserName() + ", payment of $" + billAmount + " was successful!");
		} else {
			System.out.println("Sorry " + user.getUserName() + ", you do not have enough balance to pay the bill!");
		}
		System.out.println("Your wallet balance is $" + user.getWalletBalance());

		if (user instanceof PremiumUser) {
			PremiumUser premiumUser = (PremiumUser) user;
			System.out.println("You have " + premiumUser.getRewardPoints() + " points!");
		}
		System.out.println();
    }
}



```

<img width="513" alt="Capture" src="https://user-images.githubusercontent.com/105406807/169656389-5fb4a0d7-32f3-46ae-982e-0d885e5afb33.PNG">
<img width="509" alt="Capture" src="https://user-images.githubusercontent.com/105406807/169656421-a7cd1b1e-ae28-4111-8671-b838aca5fa47.PNG">

<img width="436" alt="Capture" src="https://user-images.githubusercontent.com/105406807/169656436-f3c364f1-14cd-48f8-84bb-a88df6c47be4.PNG">



```java
public class Faculty {
	private String name;
	private float basicSalary;
	private float bonusPercentage;
	private float carAllowancePercentage;
	public Faculty(String name, float basicSalary) {
		this.name = name;
		this.basicSalary = basicSalary;
		this.bonusPercentage=4;
		this.carAllowancePercentage=2.5f;
	}
public double calculateSalary(){
		double facultySalary=
		this.getBasicSalary()*(1+(this.getBonusPercentage()/100)+(this.getCarAllowancePercentage()/100));
		this.setBasicSalary((float)facultySalary);
		return facultySalary;
		}
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}
	public float getBasicSalary() {
		return basicSalary;
	}
	public void setBasicSalary(float basicSalary) {
		this.basicSalary = basicSalary;
	}
	public float getBonusPercentage() {
		return bonusPercentage;
	}
	public void setBonusPercentage(float bonusPercentage) {
		this.bonusPercentage = bonusPercentage;
	}
	public float getCarAllowancePercentage() {
		return carAllowancePercentage;
	}
	public void setCarAllowancePercentage(float carAllowancePercentage) {
		this.carAllowancePercentage = carAllowancePercentage;
	}
	
	

}


public class OfficeStaff extends Faculty{
private String designation;

public OfficeStaff(String name, float basicSalary, String designation) {
	super(name, basicSalary);
	this.designation = designation;
}
public double calculateSalary() {
	double ap=0;
	switch (designation) {
	case "Accountant":
		ap=10000.0;
		break;
	case "Clerk":
		ap=7000.0;
		break;
		
	case "Peon":
		ap=4500.0;
		break;

	}
return super.calculateSalary()+ap;
}
public String getDesignation() {
	return designation;
}

public void setDesignation(String designation) {
	this.designation = designation;
}

}


public class Teacher extends Faculty {
	private String qualification;

	public Teacher(String name, float basicSalary, String qualification) {
		super(name, basicSalary);
		this.qualification = qualification;
	}
	public double calculateSalary() {
		double ap=0;
		switch (qualification) {
		case "Doctoral":
			ap=20000.0;
			break;
		case "Masters":
			ap=18000.0;
			break;
			
		case "Bachelors":
			ap=15500.0;
			break;
		case "Associate":
			ap=10000.0;
			break;
		}
	return super.calculateSalary()+ap;
	}
	public String getQualification() {
		return qualification;
	}

	public void setQualification(String qualification) {
		this.qualification = qualification;
	}

}



class Tester {
	public static void main(String[] args) {
		
		Teacher teacher = new Teacher("Caroline", 30500f, "Masters");
		OfficeStaff officeStaff = new OfficeStaff("James", 24000f, "Accountant");
		
		System.out.println("Teacher Details\n***************");
		System.out.println("Name: "+teacher.getName());
		System.out.println("Qualification: "+teacher.getQualification());
		System.out.println("Total salary: $" + Math.round(teacher.calculateSalary()*100)/100.0); 
		System.out.println();

		System.out.println("Office Staff Details\n***************");
		System.out.println("Name: "+officeStaff.getName());
		System.out.println("Designation: "+officeStaff.getDesignation());
		System.out.println("Total salary: $" + Math.round(officeStaff.calculateSalary()*100)/100.0); 

        //Create more objects for testing your code   

	}
}

```
# ABSTRACT CERDIT CARD AND DEBIT CARD

```JAVA

abstract public class Payment {
private int customerId;
protected String paymentId;
protected double serviceTaxPercentage;
public Payment(int customerId) {
	this.customerId = customerId;
}
public abstract double payBill(double amount);
public int getCustomerId() {
	return customerId;
}
public void setCustomerId(int customerId) {
	this.customerId = customerId;
}
public String getPaymentId() {
	return paymentId;
}
public void setPaymentId(String paymentId) {
	this.paymentId = paymentId;
}
public double getServiceTaxPercentage() {
	return serviceTaxPercentage;
}
public void setServiceTaxPercentage(double serviceTaxPercentage) {
	this.serviceTaxPercentage = serviceTaxPercentage;
}

}

public class DebitCardPayment extends Payment{
private static int counter=1000;
private double discountPercentage;

public DebitCardPayment(int customerId) {
	super(customerId);
	paymentId="D"+ ++counter;
	
}
public  double payBill(double amount) {
	double tt=0;
	if(amount<=500) {
		setServiceTaxPercentage(2.5);
	}
	else if(amount>500&&amount<=1000) {
		setServiceTaxPercentage(4);
	}
	else if(amount>1000) {
		setServiceTaxPercentage(5);
	}
	
	if(amount<=500) {
		setDiscountPercentage(1);
	}
	else if(amount>500&&amount<=1000) {
		setDiscountPercentage(2);
	}
	else if(amount>1000) {
		setDiscountPercentage(3);
	}
	
	tt =amount+amount*getServiceTaxPercentage()/100;
	double disc=amount*getDiscountPercentage()/100;
	return tt-disc;
	
	
	
}
public static int getCounter() {
	return counter;
}
public static void setCounter(int counter) {
	DebitCardPayment.counter = counter;
}
public double getDiscountPercentage() {
	return discountPercentage;
}
public void setDiscountPercentage(double discountPercentage) {
	this.discountPercentage = discountPercentage;
}

}

public class CreditCardPayment extends Payment {
	private static int counter=1000;

	public CreditCardPayment(int customerId) {
		super(customerId);
		paymentId="C"+ ++counter;
		
	}
	
	public  double payBill(double amount) {
		
		if(amount<=500) {
			setServiceTaxPercentage(3);
		}
		else if(amount>500&&amount<=1000) {
			setServiceTaxPercentage(5);
		}
		else if(amount>1000) {
			setServiceTaxPercentage(6);
		}
return amount+(amount*getServiceTaxPercentage()/100);
	}
	
	public static int getCounter() {
		return counter;
	}
	public static void setCounter(int counter) {
		CreditCardPayment.counter = counter;
	}
	

}

class Tester{
    public static void main(String args[]){
        DebitCardPayment debitCardPayment = new DebitCardPayment(101);
        double billAmount=Math.round(debitCardPayment.payBill(500)*100)/100.0;
		System.out.println("Customer Id: " + debitCardPayment.getCustomerId());
		System.out.println("Payment Id: " + debitCardPayment.getPaymentId());
		System.out.println("Service tax percentage: " + debitCardPayment.getServiceTaxPercentage());
		System.out.println("Discount percentage: " + debitCardPayment.getDiscountPercentage());
		System.out.println("Total bill amount: " + billAmount);
		
		CreditCardPayment creditCardPayment = new CreditCardPayment(102);
        billAmount=Math.round(creditCardPayment.payBill(1000)*100)/100.0;
		System.out.println("Customer Id: " + creditCardPayment.getCustomerId());
		System.out.println("Payment Id: " + creditCardPayment.getPaymentId());
		System.out.println("Service tax percentage: " + creditCardPayment.getServiceTaxPercentage());
		System.out.println("Total bill amount: " + billAmount);
    }
}
```
# mobile phone 

```java
 interface Testable {
public boolean testCompatibility();
}

 class Mobile  {
	private String name;
	private String brand;
	private String operatingSystemName;
	private String operatingSystemVersion;
	public Mobile(String name, String brand, String operatingSystemName, String operatingSystemVersion) {
		this.name = name;
		this.brand = brand;
		this.operatingSystemName = operatingSystemName;
		this.operatingSystemVersion = operatingSystemVersion;
	}
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}
	public String getBrand() {
		return brand;
	}
	public void setBrand(String brand) {
		this.brand = brand;
	}
	public String getOperatingSystemName() {
		return operatingSystemName;
	}
	public void setOperatingSystemName(String operatingSystemName) {
		this.operatingSystemName = operatingSystemName;
	}
	public String getOperatingSystemVersion() {
		return operatingSystemVersion;
	}
	public void setOperatingSystemVersion(String operatingSystemVersion) {
		this.operatingSystemVersion = operatingSystemVersion;
	}
	
}

 class SmartPhone extends Mobile implements Testable {
	private String networkGeneration;

	public SmartPhone(String name, String brand, String operatingSystemName, String operatingSystemVersion,
			String networkGeneration) {
		super(name, brand, operatingSystemName, operatingSystemVersion);
		this.networkGeneration = networkGeneration;
	}
	
public boolean testCompatibility() {
	boolean b=false;
	switch(getOperatingSystemName()) {
	case "Saturn":
		switch(networkGeneration) {
		case "3G":
			switch(getOperatingSystemVersion()) {
			case "1.1":
				b=true;
				break;
			case "1.2":
				b=true;
				break;
			case "1.3":
				b=true;
				break;
				
			}
			break;
		case "4G":
			switch(getOperatingSystemVersion()) {
			case "1.2":
				b=true;
				break;
			case "1.3":
				b=true;
				break;
		}
			break;
		case "5G":
			switch(getOperatingSystemVersion()) {
			case "1.3":
				b=true;
				break;
		}
			break;
	
	}
		break;
	case "Gara":
		switch(networkGeneration) {
		case "3G":
			switch(getOperatingSystemVersion()) {
			case "EXRT.1":
				b=true;
				break;
			case "EXRT.2":
				b=true;
				break;
			case "EXRU.1":
				b=true;
				break;
				
			}
			break;
		case "4G":
			switch(getOperatingSystemVersion()) {
			case "EXRT.2":
				b=true;
				break;
			case "EXRU.1":
				b=true;
				break;
		}
			break;
		case "5G":
			switch(getOperatingSystemVersion()) {
			case "EXRU.1":
				b=true;
				break;
		}	
}
	}
	return b;
}

public String getNetworkGeneration() {
	return networkGeneration;
}

public void setNetworkGeneration(String networkGeneration) {
	this.networkGeneration = networkGeneration;
}

}

class Tester {
	public static void main(String args[]){
		SmartPhone smartPhone = new SmartPhone("KrillinM20", "Nebula", "Saturn", "1.3", "5G");
		if(smartPhone.testCompatibility())
		    System.out.println("The mobile OS is compatible with the network generation!");
		else
		    System.out.println("The mobile OS is not compatible with the network generation!");
		
		//Create more objects for testing your code
	}
}

```


