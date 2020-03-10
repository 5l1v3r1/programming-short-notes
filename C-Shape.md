```
				C# (C-Sharp) Quick Revison Notes
				Written By : Pushpender Singh
```

## Intro

* C# is an object-oriented programming language created by Microsoft that runs on the .NET Framework.

## Installation

1. Install Visual Studio Community (It is a IDE--> Integrated Development Environment)
   URL: https://visualstudio.microsoft.com/vs/community/
   
2. Refer Installation : https://www.w3schools.com/cs/cs_getstarted.asp

## HelloWorld Program In C#
```
using System;

namespace HelloWorld
{
	class Program
	{
		static void Main(string[] args)
		{
			Console.WriteLine("HelloWorld");
		}
	}
}
```

## Syntax (HelloWorld Program Explanation)

* `using System;` : 
	* Importing the classes of System namespace
	
* `namespace`     : 

	* Creating Namespace,
	* Used to Organise Code, 
	* Namespace is a container of Classes & Other Namespaces
	
* `{} ` :
	* Curly Braces, Marks the BEGINNING & the END of a block of code.
	
* `class` :
	* Type of container,
	* Every Line of Code That Runs in C# is placed inside class,
	* Container of DATA & METHODS
	
* `Main `  : 
	* A METHOD,
        * Anything inside it is executed
	 (It is Discussed In Detail Below)
	 
* `Console.WriteLine() ` : 
	* Console is a CLASS of SYSTEM namespace,
	* Use to Print/Write/Output the text/string	
	* If we don't use "using System;" then we can write it like this:
	   `System.Console.WriteLine()`
							   
* `WriteLine()` :
	* Use to Write text in console in New Line
	
* `Write()` :
	* Use to Write text in console in Same Line
	
* `;`  : 
	* Each Line is ended with semi-colon (;)

### Note: C# is case-sensitive: "MyClass" and "myclass" has different meaning.

## Difference b/w WriteLine() & Write() METHODS
```	
	* CODE EXAMPLE:
	---------------
	
	Console.WriteLine("Hello World!");  
	Console.WriteLine("I will print on a new line.");

	Console.Write("Hello World! ");
	Console.Write("I will print on the same line."); 
```
```
	* RESULT:
	---------
	Hello World!
	I will print on a new line.
	Hello World! I will print on the same line.
```

## Comments In C#
* Code Which is Ignored my the Compiler (of C#), as is coded To Increase the readibilty of code

### Types :

* `Single Liner`: Start with two forward slashes (//)

```
   	-------------------------------------
	* Example of Single Liner Comments :
	-------------------------------------
	// I am Single Liner Comment, & will be Ignored by the C# 
	Console.WriteLine("Hello World!");    // This Line Will Print "Hello World!" In Console
```
```
	----------
	* RESULT :
	----------
	Hello World!
```

* Multi Liner: Start with /* and ends with */
```  
	-------------------------------------
	* Example of Multi Liner Comments :
	-------------------------------------
	/* I am Multi Liner Comment, & will be Ignored by the C# 
	   Below Line Will Print "Hello World!" In Console  */
	Console.WriteLine("Hello World!");    
```
```
	----------
	* RESULT :
	----------
	Hello World
```

### NOTE: Single-Liner Comment is used to comment out single line & To comment multiple lines, we use Multi-Liner Comment. 
	
## Variables In C#
* Variables are containers for storing data values.

* Diffent Types of Variables (defined with different keywords):
	* int    - stores integers (whole numbers), without decimals, such as 123 or -123
	* double - stores floating point numbers, with decimals, such as 19.99 or -19.99
	* char   - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes  
	* string - stores text, such as "Hello World". String values are surrounded by double quotes
	* bool   - stores values with two states: true or false

* Declaring (Creating) Variables:
	* To create a variable, you must specify the type and assign it a value:
	```
	Syntax:  datatype variableName = value; 
	        datatype      ==> int, double, string, bool, char
	        variableName  ==> Can be Anything
	        =             ==> Single Equal Sign (=) is used to assign value
	```
	
	```
	=======================================
	* EXAMPLE (Storing String In Variable):
	=======================================
	string name = "Pushpender";
	Console.WriteLine(name);
	
	----------
	* RESULT:
	----------
	'Pushpender'
	```
	
	```
	========================================
	* EXAMPLE (Storing Integer In Variable):
	========================================
	int myNumber = 10;
	Console.WriteLine(myNumber);
	
	----------
	* RESULT:
	----------
	10
	```
	```
	========================================
	* EXAMPLE (Storing Double In Variable):
	========================================
	double myDecimalInteger = 10.2;
	Console.WriteLine(myDecimalInteger);
	
	----------
	* RESULT:
	----------
	10.2
	```
	```
	========================================
	* EXAMPLE (Storing Character In Variable):
	========================================
	char myChar = 'a';
	Console.WriteLine(myChar);
	
	----------
	* RESULT:
	----------
	'a'
	```
	```
	========================================
	* EXAMPLE (Storing Boolean In Variable):
	========================================
	bool male = true;
	Console.WriteLine(male);
	
	----------
	* RESULT:
	----------
	true
	```


	
	

	
	
	


	
	
	
	



