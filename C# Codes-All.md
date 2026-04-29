**C# Codes:-**



//Sum of 2 nums

using System;

namespace Program1{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           Console.WriteLine("Hi");

&#x20;           //Sum of 2 nums

&#x20;           Console.WriteLine("Enter 2 nums:");

&#x20;           int a,b,s;

&#x20;           a=Convert.ToInt32(Console.ReadLine());

&#x20;           b=Convert.ToInt32(Console.ReadLine());

&#x20;           s=a+b;

&#x20;           Console.WriteLine("Sum of {0}, {1}: {2}",a,b,s);

&#x20;

&#x20;       }

&#x20;   }

}



\-------------------------------------------------------------------------------------------------------------------------------------

//Vote or not?

using System;

namespace Program2{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           int age,d;

&#x20;           Console.Write("Enter age:");

&#x20;           age=Convert.ToInt32(Console.ReadLine());

&#x20;           if(age>=18){

&#x20;               Console.Write("Eligible to Vote.");

&#x20;           }

&#x20;           else{

&#x20;               Console.WriteLine("Not eligible to Vote.");

&#x20;               d=18-age;

&#x20;               Console.WriteLine("Need to wait for {0} years to vote.",d);

&#x20;           }

&#x20;       }

&#x20;   }

}

\----------------------------------------------------------------------------------------------------------------------------------------

//calculator-SWITCH CASE

using System;

namespace Program3{

&#x20;   class Calculator{

&#x20;       public static void Main(String\[] args){

&#x20;           int a,b;

&#x20;           Console.WriteLine("Enter 2 nums:");

&#x20;           a=Convert.ToInt32(Console.ReadLine());

&#x20;           b=Convert.ToInt32(Console.ReadLine());

&#x20;           char op;

&#x20;           Console.WriteLine("Enter operator (+,-,\*,/):");

&#x20;           op=Convert.ToChar(Console.ReadLine());

&#x20;           if(op=='+' || op=='-' || op=='\*' || op=='/'){

&#x20;               switch(op){

&#x20;                   case '+':

&#x20;                   Console.WriteLine("Sum={0}",a+b);

&#x20;                   break;

&#x20;                   case '-':

&#x20;                   Console.WriteLine("Difference={0}",a-b);

&#x20;                   break;

&#x20;                   case '\*':

&#x20;                   Console.WriteLine("Multiply={0}",a\*b);

&#x20;                   break;

&#x20;                   case '/':

&#x20;                   if(a>b){

&#x20;                       Console.WriteLine("Division={0}",a/b);

&#x20;                       break;

&#x20;                   }else if(b>a){

&#x20;                       Console.WriteLine("Division={0}",b/a);

&#x20;                       break;

&#x20;                   }

&#x20;                   else{

&#x20;                       Console.WriteLine("Invalid Input");

&#x20;                       break;

&#x20;                   }

&#x20;

&#x20;                   default:

&#x20;                   Console.WriteLine("Invalid");

&#x20;                   break;

&#x20;               }

&#x20;           }

&#x20;       }

&#x20;   }

}

\----------------------------------------------------------------------------------------------------------------------------------------

//Print natural numbers-for loop

using System;

namespace Program4{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           int i,n;

&#x20;           Console.WriteLine("Print natural nums(limit):");

&#x20;           n=Convert.ToInt32(Console.ReadLine());

&#x20;           Console.WriteLine("Natural numbers are ");

&#x20;           for(i=1;i<=n;i++){

&#x20;               Console.Write("{0}, ",i);

&#x20;           }

&#x20;       }

&#x20;   }

}

\----------------------------------------------------------------------------------------------------------------------------------------

//Factorial->while-loop

using System;

namespace Program5{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           int i,fact=1;

&#x20;           Console.WriteLine("Enter num(Factorial):");

&#x20;           i=Convert.ToInt32(Console.ReadLine());

&#x20;           while(i>0){

&#x20;               fact=fact\*i;

&#x20;               i--;

&#x20;           }

&#x20;           Console.WriteLine("Factorial: {0}",fact);

&#x20;       }

&#x20;   }

}

\----------------------------------------------------------------------------------------------------------------------------------------

//Incremental or Decremental operator

using System;

namespace Program6{

class Basic

{

&#x20;   static public void Main()

&#x20;   {

&#x20;       int a = 5;

&#x20;     	// pre-increment

&#x20;       Console.WriteLine("++a returns: " + ++a);

&#x20;     	// post-increment

&#x09;Console.WriteLine("a++ returns: " + a++);

&#x20;     	Console.WriteLine("Final value of a: " + a);

&#x20;

&#x20;     	Console.WriteLine();

&#x20;

&#x20;       // pre-decrement

&#x20;     	Console.WriteLine("--a returns: " + --a);

&#x20;

&#x20;     	// post-decrement

&#x20;     	Console.WriteLine("a-- returns: " + a--);

&#x20;

&#x20;     	Console.WriteLine("Final value of a: " + a);

&#x20;   }

&#x20; }

}

\----------------------------------------------------------------------------------------------------------------------------------------

**ARRAYS CODES:**

//Arrays

using System;

namespace Program7{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           int\[] arr1;

&#x20;           arr1=new int\[5];

&#x20;           arr1\[0]=0;

&#x20;           arr1\[1]=1;

&#x20;           arr1\[2]=2;

&#x20;           arr1\[3]=3;

&#x20;           arr1\[4]=4;

&#x20;           //Print elements of array

&#x20;           Console.Write("Array elements:\\n");

&#x20;           for(int i=0;i<5;i++){

&#x20;               Console.Write(arr1\[i]+" ");

&#x20;           }

&#x20;       }

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Sum \& avg of array elements:

using System;

namespace ArrayBasics{

&#x20; class Program{

&#x20;   public static void Main(String\[] args){

&#x20;     Console.WriteLine("Enter size of array:");

&#x20;     int n=Convert.ToInt32(Console.ReadLine());

&#x20;     int\[] arr=new int\[n];

&#x20;     Console.WriteLine("Enter elements of array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       arr\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;     }

&#x20;     Console.WriteLine("Array:");

&#x20;     int sum=0;

&#x20;     for(int i=0;i<n;i++){

&#x20;       Console.Write("{0} ",arr\[i]);

&#x20;       sum+=arr\[i];

&#x20;     }

&#x20;     double avg =(double)sum/n;

&#x20;     Console.WriteLine("\\nSum of array elements is {0}",sum);

&#x20;     Console.WriteLine("\\nAverage of array elements is {0}",avg);

&#x20;   }

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Days in a week ,string array->foreach loop used

using System;

namespace Program8{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           string\[] weekDays;

&#x20;           weekDays=new\[] {"Sun","Mon", "Tue", "Wed","Thu", "Fri", "Sat"};

&#x20;           Console.WriteLine("Days in a Week:");

&#x20;           foreach(string day in weekDays){

&#x20;               Console.Write(day+" ");

&#x20;           }

&#x20;       }

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Sorted numbers in array

using System;

namespace Program9{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           int\[] arr1={13,57,9,24,68};

&#x20;           int temp;

&#x20;           Console.WriteLine("Array Elements:");

&#x20;           foreach(int num in arr1){

&#x20;               Console.Write(num+" ");

&#x20;           }

&#x20;           for(int i=0;i<5;i++){

&#x20;               for(int j=0;j<i;j++){

&#x20;                   if(arr1\[j]>arr1\[j+1]){

&#x20;                       temp=arr1\[j];

&#x20;                       arr1\[j]=arr1\[j+1];

&#x20;                       arr1\[j+1]=temp;

&#x20;                   }

&#x20;               }

&#x20;           }

&#x20;           Console.WriteLine("\\nSorted Array Elements:");

&#x20;           foreach(int num in arr1){

&#x20;               Console.Write(num+" ");

&#x20;           }

&#x20;       }

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//largest,smallest in array

using System;

namespace ArrayBasics{

&#x20; class Program{

&#x20;   public static void Main(String\[] args){

&#x20;     Console.WriteLine("Enter size of array:");

&#x20;     int n=Convert.ToInt32(Console.ReadLine());

&#x20;     int\[] arr=new int\[n];

&#x20;     Console.WriteLine("Enter elements of array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       arr\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;     }

&#x20;     Console.WriteLine("Array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       Console.Write("{0} ",arr\[i]);

&#x20;     }

&#x20;     int min=arr\[0];

&#x20;     int max=arr\[0];

&#x20;     for(int i=0;i<n;i++){

&#x20;       if(arr\[i]>max){

&#x20;         max=arr\[i];

&#x20;       }

&#x20;       if(arr\[i]<min){

&#x20;         min=arr\[i];

&#x20;       }

&#x20;     }

&#x20;     Console.WriteLine("Min: {0}, Max: {1}",min,max);

&#x20;   }

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Reverse array

using System;

namespace Program11{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           int size;

&#x20;           Console.Write("Enter size of array:");

&#x20;           size=Convert.ToInt32(Console.ReadLine());

&#x20;           int\[] arr=new int\[size];

&#x20;           Console.WriteLine("Enter elements of array:");

&#x20;           for(int i=0;i<size;i++){

&#x20;               arr\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;           }

&#x20;           Console.WriteLine("\\nOriginal array:");

&#x20;           foreach (int num in arr){

&#x20;               Console.Write(num+", ");

&#x20;           }



&#x20;           Console.WriteLine("\\nReversed array:");

&#x20;           for(int i=size-1;i>=0;i--){

&#x20;               Console.Write(arr\[i]+" ");

&#x20;           }

&#x20;       }

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Count of even and odd in array:

using System;

namespace ArrayBasics{

&#x20; class Program{

&#x20;   public static void Main(String\[] args){

&#x20;     Console.WriteLine("Enter size of array:");

&#x20;     int n=Convert.ToInt32(Console.ReadLine());

&#x20;     int\[] arr=new int\[n];

&#x20;     Console.WriteLine("Enter elements of array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       arr\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;     }

&#x20;     Console.WriteLine("Array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       Console.Write("{0} ",arr\[i]);

&#x20;     }

&#x20;     int even=0;

&#x20;     int odd=0;

&#x20;     for(int i=0;i<n;i++){

&#x20;       if(arr\[i]%2==0){

&#x20;         even++;

&#x20;       }

&#x20;       else{

&#x20;         odd++;

&#x20;       }

&#x20;     }

&#x20;     Console.WriteLine("Count of Even's:{0}, Odd's:{1}",even,odd);

&#x20;   }

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Search num in array:
using System;

namespace ArrayBasics{

&#x20; class Program{

&#x20;   public static void Main(String\[] args){

&#x20;     Console.WriteLine("Enter size of array:");

&#x20;     int n=Convert.ToInt32(Console.ReadLine());

&#x20;     int\[] arr=new int\[n];

&#x20;     Console.WriteLine("Enter elements of array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       arr\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;     }

&#x20;     Console.WriteLine("Array:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       Console.Write("{0} ",arr\[i]);

&#x20;     }

&#x20;     bool found=false;

&#x20;     int key=Convert.ToInt32(Console.ReadLine());

&#x20;     for(int i=0;i<n;i++){

&#x20;       if(arr\[i]==key){

&#x20;         Console.WriteLine("Element found at {0} index, {1} position",i,i+1);

&#x20;         found=true;

&#x20;         break;

&#x20;       }

&#x20;     }

&#x20;     if(!found){

&#x20;       Console.WriteLine("Element not found!");

&#x20;     }

&#x20;   }

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Copy 1 array to another

using System;

namespace CopyArray{

&#x20; class Program{

&#x20;   public static void Main(String\[] args){

&#x20;     Console.WriteLine("Enter size of array:");

&#x20;     int n=Convert.ToInt32(Console.ReadLine());

&#x20;     int\[] a= new int\[n];

&#x20;     int\[] b=new int\[n];

&#x20;     Console.WriteLine("Enter {0} elements of array:",n);

&#x20;     for(int i=0;i<n;i++){

&#x20;       a\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;       b\[i]=a\[i];

&#x20;     }

&#x20;     Console.WriteLine("Array1:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       Console.Write(a\[i]+" ");

&#x20;     }

&#x20;     Console.WriteLine("\\nArray2:");

&#x20;     for(int i=0;i<n;i++){

&#x20;       Console.Write(b\[i]+" ");

&#x20;     }

&#x20;   }

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//print repeating elements in array

using System;

class Program

{

&#x20;   static void Main()

&#x20;   {

&#x20;     Console.WriteLine("Enter size of array:");

&#x20;     int n=Convert.ToInt32(Console.ReadLine());

&#x20;     int\[] arr=new int\[n];

&#x20;     Console.WriteLine("Enter array elements:");

&#x20;     for(int i=0;i<n;i++)

&#x20;     {

&#x20;         arr\[i]=Convert.ToInt32(Console.ReadLine());

&#x20;     }

&#x20;     Console.WriteLine("Repeating elements:");

&#x20;     for (int i=0;i<n;i++)

&#x20;     {

&#x20;       for (int j=i+1;j<n;j++)

&#x20;       {

&#x20;         if (arr\[i]==arr\[j])

&#x20;         {

&#x20;           Console.WriteLine(arr\[i]);

&#x20;           break;

&#x20;         }

&#x20;       }

&#x20;     }

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

Factorial using function:
using System;

class Program{

&#x20; static void Factorial(int m){

&#x20;   int d=1;

&#x20;   for(int i=1;i<=m;i++){

&#x20;     d=d\*i;

&#x20;   }

&#x20;   Console.WriteLine("Factorial of {0} is {1}",m,d);

&#x20; }

&#x20; public static void Main(String\[] args){

&#x20;   int n=5;

&#x20;   Factorial(n);

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Fibonacci using function

using System;

class Program

{

&#x20;   static void Fibonacci(int n)

&#x20;   {

&#x20;       int a=0,b=1,c;

&#x20;       Console.WriteLine("Fibonacci Series:");

&#x20;       Console.Write(a+" "+b+" ");

&#x20;       for(int i=2;i<n;i++)

&#x20;       {

&#x20;           c=a+b;

&#x20;           Console.Write(c+" ");

&#x20;           a=b;

&#x20;           b=c;

&#x20;       }

&#x20;   }

&#x20;   static void Main()

&#x20;   {

&#x20;       Console.WriteLine("Enter number of terms:");

&#x20;       int n = Convert.ToInt32(Console.ReadLine());

&#x20;       Fibonacci(n);   // function call

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

**STRING CODES:**

//String-i/p,o/p

using System;

namespace Program12{

&#x20;   class Basic{

&#x20;       public static void Main(String\[] args){

&#x20;           string qw;

&#x20;           Console.WriteLine("Enter string:");

&#x20;           qw=Console.ReadLine();

&#x20;           Console.WriteLine("Given string: "+qw);



&#x20;           string v="Hello Wolrd";

&#x20;           foreach(char r in v){

&#x20;           Console.Write(r);

&#x20;           }

&#x20;       }

&#x20;   }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//print string \& it's length , reverse string, convert to lower \& upper

using System;

class Program{

&#x20; public static void Main(String\[] args){

&#x20;   Console.WriteLine("Enter string:");

&#x20;   string str=Console.ReadLine();

&#x20;   Console.WriteLine(str+" Length is {0}",str.Length);

&#x20;   Console.WriteLine("Reverse string:");

&#x20;   for(int i=str.Length-1;i>=0;i--)

&#x20;   {

&#x20;     Console.Write(str\[i]);

&#x20;   }

&#x20;   Console.WriteLine("Uppercase: " + str.ToUpper());

&#x20;   Console.WriteLine("Lowercase: " + str.ToLower());

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//Palindrome string:
using System;

class Program{

&#x20; public static void Main(String\[] args){

&#x20;   string str="madam";

&#x20;   string rev="";

&#x20;   for(int i=str.Length-1;i>=0;i--){

&#x20;     rev+=str\[i];

&#x20;   }

&#x20;   if(rev==str){

&#x20;     Console.WriteLine("Palindrome string");

&#x20;   }

&#x20;   else{

&#x20;     Console.WriteLine("Not palindrome string");

&#x20;   }

&#x20; }

}

\---------------------------------------------------------------------------------------------------------------------------------------

//All rounder code for strings:
using System;

class Program

{

&#x20;   public static void Main()

&#x20;   {

&#x20;       string str="Hello World good morning";



&#x20;       // 1. Count vowels

&#x20;       int vowelCount = 0;

&#x20;       string lowerStr = str.ToLower();



&#x20;       for (int i = 0; i < lowerStr.Length; i++)

&#x20;       {

&#x20;           char ch = lowerStr\[i];

&#x20;           if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u')

&#x20;               vowelCount++;

&#x20;       }



&#x20;       // 2. Count words

&#x20;       string\[] words = str.Split(' ');

&#x20;       int wordCount = words.Length;



&#x20;       // 3. Replace a word

&#x20;       Console.WriteLine("Enter word to replace:");

&#x20;       string oldWord = Console.ReadLine();



&#x20;       Console.WriteLine("Enter new word:");

&#x20;       string newWord = Console.ReadLine();



&#x20;       string replacedStr = str.Replace(oldWord, newWord);



&#x20;       // 4. Some useful string methods

&#x20;       Console.WriteLine();

&#x20;       Console.WriteLine("Vowel count: " + vowelCount);

&#x20;       Console.WriteLine("Word count: " + wordCount);

&#x20;       Console.WriteLine("Replaced string: " + replacedStr);

&#x20;       Console.WriteLine("Uppercase: " + str.ToUpper());

&#x20;       Console.WriteLine("Lowercase: " + str.ToLower());

&#x20;       Console.WriteLine("Length of string: " + str.Length);

&#x20;   }

}

\-----------------------------------------------------------------------------------------------------------------------------------------------------------

\-----------------------------------------------------------------------------------------------------------------------------------------------------------

OOPS Concept:

1\. Class

A class is a blueprint that defines properties (data) and methods (behavior) of an object.



2\. Object

An object is an instance of a class that represents a real-world entity.



3\. Encapsulation

Encapsulation is the process of hiding data and allowing access through controlled methods.



4\. Inheritance

Inheritance allows one class to acquire the properties and methods of another class.



5\. Polymorphism

Polymorphism allows the same method to behave differently based on the object.



6\. Abstraction

Abstraction hides implementation details and shows only the essential features.



\-----------------------------------------------------------------------------------------------------------------------------------------------------------

\-----------------------------------------------------------------------------------------------------------------------------------------------------------

using System;



// ----- Encapsulation -----

public class Animal

{

&#x20;   // Private field (encapsulation)

&#x20;   private string name;



&#x20;   // Public property to access private field

&#x20;   public string Name

&#x20;   {

&#x20;       get { return name; }

&#x20;       set { name = value; }

&#x20;   }



&#x20;   // Virtual method (for polymorphism)

&#x20;   public virtual void Speak()

&#x20;   {

&#x20;       Console.WriteLine("Animal makes a sound.");

&#x20;   }

}



// ----- Inheritance -----

public class Dog : Animal

{

&#x20;   // Override method (polymorphism)

&#x20;   public override void Speak()

&#x20;   {

&#x20;       Console.WriteLine("Dog barks: Woof Woof!");

&#x20;   }

}



// ----- Abstraction -----

public abstract class Shape

{

&#x20;   public abstract void Draw();

}



public class Circle : Shape

{

&#x20;   public override void Draw()

&#x20;   {

&#x20;       Console.WriteLine("Drawing a Circle");

&#x20;   }

}



// ----- Main Program -----

public class Program

{

&#x20;   public static void Main()

&#x20;   {

&#x20;       // Object creation

&#x20;       Dog myDog = new Dog();

&#x20;       myDog.Name = "Buddy";

&#x20;       Console.WriteLine($"Dog Name: {myDog.Name}");

&#x20;       myDog.Speak();  // Polymorphism



&#x20;       Shape shape = new Circle();

&#x20;       shape.Draw();   // Abstraction

&#x20;   }

}

