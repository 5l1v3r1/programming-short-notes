```
				C# (C-Sharp) Quick Revison Notes
				Written By : Pushpender Singh
```

# Table of Context

* [Intro](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#intro)
* [Installation](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#installation)
* [HelloWorld Program In C#](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#helloworld-program-in-c)
* [Syntax (HelloWorld Program Explanation)](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#syntax-helloworld-program-explanation)
* [Comments In C#](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#comments-in-c)
* [Variables In C#](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#variables-in-c)
   * [Constant](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#constant)
   * [Concatination of String Variable & Displaying the Result](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#concatination-of-string-variable--displaying-the-result)
   * [Declaring Multiple Keywords In One Line](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#declaring-multiple-keywords-in-one-line)
   * [Identifiers In C#](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#identifiers-in-c)
   * [Naming Convention of Variables](https://github.com/Technowlogy-Pushpender/programming-short-notes/blob/master/C-Shape.md#naming-convention-of-variables)
* [DataTypes In C#]()   

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
	* Console is a **class** of **System** namespace,
	* Use to Print/Write/Output the text/string	
	* If we don't use `using System;` then we can write it like this:
	   `System.Console.WriteLine()`
							   
* `WriteLine()` :
	* Use to Write text in console in New Line
	
* `Write()` :
	* Use to Write text in console in Same Line
	
* `;`  : 
	* Each Line is ended with semi-colon (;)

#### Note: C# is case-sensitive: "MyClass" and "myclass" has different meaning.

#### Difference b/w WriteLine() & Write() METHODS
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
* Code Which is Ignored my the Compiler (of C#), and is coded To Increase the readibilty of code

#### Types :

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

#### NOTE: Single-Liner Comment is used to comment out single line & To comment multiple lines, we use Multi-Liner Comment. 
	
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

#### Constant
* A keyword which is used to make a variable read-only, immutable (*cannot change*)
* Syntax:
```
const string Author = "Pushpender";
```
* If you try to change *Constant Variables* like this,
```
Author = "Thanos";  //You Will Get Error
```
	
#### Note: 
* `Constant Variable` are defined by the User, they can be of any datatype such as `int`, `char`, etc
* They can't be declared without assigning a value
```
const string Author;
Author = "Pushpender";   // Error
```

#### Concatination of String Variable & Displaying the Result
* Code Snippet
```
string name = "Pushpender";
Console.WriteLine("Hello " + name + "!");
```
* Result
```
Hello Pushpender!
```

#### Note: `+` is a Arithmetic Operator which can be used multiple times (`Will Discuss More About Operators`)

* Code Snippet 
```
// Example of Concatenation of Two Variable Values of string Datatype
string firstName = "Pushpender";   // Storing Value of string Datatype
string lastName = "Singh";         // Storing Value of string Datatype
Console.WriteLine("Hello " + firstName + " " + lastName);       // Writing the result on Coonsole
```
* Result
```
Hello Pushpender Singh
```

* Code Snippet 
```
// Example of Concatenation of Two Variable Values of int Datatype
int firstNumber = 10;   	// Storing Value of int Datatype
string secondNumber = 20;       // Storing Value of int Datatype
Console.Write("Sum of 1st & 2nd Number is ");
Console.Write(firstNumber + secondNumber);       // Writing the result on Coonsole
```
* Result
```
Sum of 1st & 2nd Number is 30
```

#### Declaring Multiple Keywords In One Line
* `Comma`(,) can be used to declare multiple values of **same datatype** In One Line
* Code Snippet
```
int x = 10, y = 20, z = 30;
Console.WriteLine(x + y + z);
```

* Result
```
60
```

#### Identifiers In C#
* In Any Programming Language, variable name should be unique, or **variables** should be **identified** by **Unique Names**
* Thus **Unique Names** are known as **Identifiers**

* Typically, one can name the variables as *x*, *y*, *z* but it is not a good practice.
* `Meaningful Descriptive names` such as `Author`, `PlayerName`, `GunName` etc should be used in a program to increase the readability of code.

#### Naming Convention of Variables
* Essential Rules for Naming Variables In C#
   * Should Not Starts With Number & can starts with underscore (_)
   * Variable Name can only starts with a *number* or *underscore*
   * Should Starts with `lowercase` letter and `whitespaces` are prohibited
   * Variable Names are case-sensitive which means that `MyName` & `myName` are two different words
   * `Reserve Keywords`/`Keywords In C#` (*which are meaningful to the compiler*)  such as `int`, `string`, etc can't be used as Variable Name
   * Should Not Contain a DOT (.) , for e.g. `D.O.B` can't be used as Varible, but `DOB` can be used as Variable Name
   
## DataTypes In C#


	


	
	
	
	



