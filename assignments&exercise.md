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





