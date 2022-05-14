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
![Capture](https://user-images.githubusercontent.com/105406807/168332641-d65bb10d-fe93-4d46-9d7d-01c9af4b9375.PNG)
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

