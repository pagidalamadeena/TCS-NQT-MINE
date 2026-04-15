**----:JAVA:---------**

Basic input:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       System.out.print("Enter Name:");

&#x20;       String name=sc.nextLine();

&#x20;       System.out.print("Enter age:");

&#x20;       int age=sc.nextInt();

&#x20;       System.out.print("Enter salary:");

&#x20;       double sal=sc.nextDouble();

&#x20;       System.out.println("Name:"+name+" Age:"+age+" Salary:"+sal);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

if-else:

import java.util.Scanner;

class Program1{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       System.out.print("Enter score:");

&#x20;       int s=sc.nextInt();

&#x20;       if(s>=51 \&\& s<=100){

&#x20;           System.out.println("Pass");

&#x20;       }

&#x20;       else if(s<=50 \&\& s>=0){

&#x20;           System.out.println("Fail");

&#x20;       }

&#x20;       else{

&#x20;           System.out.println("Invalid Score!");

&#x20;       }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Switch case:
import java.util.Scanner;

class Program1{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter 2 nums:");

&#x20;       int a=sc.nextInt();

&#x20;       int b=sc.nextInt();

&#x20;       System.out.print("Enter Operator(+ - \* /):");

&#x20;       char c=sc.next().charAt(0);

&#x20;       System.out.print("Answer:");

&#x20;       switch(c){

&#x20;           case '+':

&#x20;               System.out.print(a+b);

&#x20;               break;

&#x20;           case '-':

&#x20;               System.out.print(a-b);

&#x20;               break;

&#x20;           case '\*':

&#x20;               System.out.print(a\*b);

&#x20;               break;

&#x20;           case '/':

&#x20;               if(a>b){

&#x20;                   System.out.print(a/b);

&#x20;                   break;

&#x20;               }

&#x20;               else{

&#x20;                   System.out.print(b/a);

&#x20;                   break;

&#x20;               }

&#x20;           default:

&#x20;           System.out.println("Invalid Input");

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Constant(final):

public class Constant1 {

&#x20;   public static void main(String\[] args) {

&#x20;       final int MAX = 100;

&#x20;       System.out.println(MAX);

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Strings-Basic-Keywords also:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       System.out.print("Enter word/line:");

&#x20;       String str=sc.nextLine();

&#x20;

&#x20;       //count no.of chars

&#x20;       System.out.println("No.of chars: "+str.length());

&#x20;

&#x20;       //char at index(0-4)

&#x20;       System.out.println("Char at index: "+str.charAt(1));

&#x20;

&#x20;       //toUpperCase, toLowerCase

&#x20;       System.out.println("Uppercase: "+str.toUpperCase());

&#x20;       System.out.println("Lowercase: "+str.toLowerCase());

&#x20;

&#x20;       //Equal or not? .equals()

&#x20;       String a="java";

&#x20;       String b="Java";

&#x20;       System.out.println("Check case: "+a.equals(b));

&#x20;

&#x20;       //Equal or not, ignorecase

&#x20;       System.out.println("Check case: "+a.equalsIgnoreCase(b));

&#x20;

&#x20;       // contains

&#x20;       String str1="java programming is good";

&#x20;       System.out.println("Substring is there/not: "+str1.contains("good"));

&#x20;

&#x20;       // substring()

&#x20;       System.out.println("Substring taken: "+str1.substring(0,3));

&#x20;

&#x20;       //replace()

&#x20;       System.out.println(str1.replace('g','h'));

&#x20;

&#x20;       //trim()- removes extra spaces

&#x20;       String we="     Madeena   ";

&#x20;       System.out.println(we.trim());

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

print all char of string:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String str=sc.nextLine();

&#x20;       for(int i=0;i<str.length();i++){

&#x20;           System.out.println(str.charAt(i));

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

count vowels in string:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;   Scanner sc=new Scanner(System.in);

&#x20;   System.out.print("Enter string:");

&#x20;   String str=sc.nextLine();

&#x20;   int count=0;

&#x20;   for(int i=0;i<str.length();i++){

&#x20;       char m=str.charAt(i);

&#x20;       if(m=='a' ||m=='e' ||m=='i' ||m=='o' ||m=='u' ||m=='A' ||m=='E' ||m=='I' ||m=='O' ||m=='U'){

&#x20;           count++;

&#x20;       }

&#x20;   }

&#x20;   System.out.print("No.of vowels: "+count);

&#x20;   sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Reverse string:
//Reverse a string

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String str=sc.nextLine();

&#x20;       int l=str.length();

&#x20;       for(int i=l-1;i>=0;i--){

&#x20;           System.out.println(str.charAt(i));

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Palindrome string:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String str=sc.nextLine();

&#x20;       int l=str.length();

&#x20;       String rev="";

&#x20;       for(int i=l-1;i>=0;i--){

&#x20;           //System.out.println(str.charAt(i));    ->print reverse string

&#x20;           rev=rev+ str.charAt(i);

&#x20;       }

&#x20;       if(str.equals(rev)){

&#x20;           System.out.print("Palindrome string");

&#x20;       }

&#x20;       else{

&#x20;           System.out.print("Not Palindrome string");

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Count no.of words in string:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String str=sc.nextLine();

&#x20;       String\[] words=str.split(" ");

&#x20;       System.out.print("No.of word: "+words.length);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Count uppercase, lowercase, digits, spaces:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String str=sc.nextLine();

&#x20;       int uc=0, lc=0, spaces=0, dg=0;

&#x20;       int l=str.length();

&#x20;       for(int i=0;i<l;i++){

&#x20;           char c=str.charAt(i);

&#x20;           if(c>='A' \&\& c<='Z'){

&#x20;               uc++;

&#x20;           }else if(c>='a' \&\& c<='z'){

&#x20;               lc++;

&#x20;           }else if(c>='0' \&\& c<='9'){

&#x20;               dg++;

&#x20;           }else{

&#x20;               spaces++;

&#x20;           }

&#x20;       }

&#x20;       System.out.println("Uppercase: "+uc);

&#x20;       System.out.println("Lowercase: "+lc);

&#x20;       System.out.println("Digits: "+dg);

&#x20;       System.out.println("Spaces: "+spaces);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Replace vowels with '\*' in string:

class Program {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       System.out.print("Enter string: ");

&#x20;       String str = sc.nextLine();

&#x20;       StringBuilder result = new StringBuilder();

&#x20;       for (int i = 0; i < str.length(); i++) {

&#x20;           char c = str.charAt(i);

&#x20;           if (c=='a'||c=='e'||c=='i'||c=='o'||c=='u' || c=='A'||c=='E'||c=='I'||c=='O'||c=='U') {

&#x20;               result.append('\*');

&#x20;           } else {

&#x20;               result.append(c);

&#x20;           }

&#x20;       }

&#x20;       System.out.println("Modified string: " + result);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

class RemoveSpaces {

&#x20;   public static void main(String\[] args) {

&#x20;       String s = "Java Programming Language";

&#x20;       System.out.println(s.replace(" ", ""));

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Remove duplicates from string:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String s=sc.nextLine();

&#x20;       String result="";

&#x20;       for(int i=0;i<s.length();i++){

&#x20;           if(!result.contains(""+s.charAt(i))){

&#x20;               result+=s.charAt(i);

&#x20;           }

&#x20;       }System.out.println(result);

&#x20;   }

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Remove vowels from string:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;       System.out.print("Enter string:");

&#x20;       String str=sc.nextLine();

&#x20;       String str1=str.replaceAll("\[AEIOUaeiou]","");

&#x20;       System.out.print("String without vowel: "+str1);

&#x20;   }

}                                                                    OR

import java.util.Scanner;

class Program {

&#x20;   public static void main(String\[] args) {

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       System.out.print("Enter a string: ");

&#x20;       String str = sc.nextLine();

&#x20;       StringBuilder result = new StringBuilder();

&#x20;       for (int i = 0; i < str.length(); i++) {

&#x20;           char c = str.charAt(i);

&#x20;           // Check if character is NOT a vowel

&#x20;           if (! (c=='a' || c=='e' || c=='i' || c=='o' || c=='u' ||c=='A' || c=='E' || c=='I' || c=='O' || c=='U') ) {

&#x20;               result.append(c);

&#x20;           }

&#x20;       }

&#x20;       System.out.println("String after removing vowels: " + result);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

\------------------------------------------------------------------------------------------------------------------------------------------------------------

**Arrays:**

Basic array input:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter size of array:");

&#x20;       int n=sc.nextInt();

&#x20;       int\[] arr = new int\[n];

&#x20;       System.out.print("Enter elements of array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           arr\[i]=sc.nextInt();

&#x20;       }

&#x20;       System.out.println("Array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           System.out.println(arr\[i]);

&#x20;       }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Min Max in array:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;       System.out.print("Enter size:");

&#x20;       int n=sc.nextInt();

&#x20;       int\[] arr=new int\[n];

&#x20;       System.out.print("Enter elements:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           arr\[i]=sc.nextInt();

&#x20;       }

&#x20;       System.out.print("Array: ");

&#x20;       for(int i=0;i<n;i++){

&#x20;           System.out.print(arr\[i]+" ");

&#x20;       }

&#x20;       int min=arr\[0];

&#x20;       int max=arr\[0];

&#x20;       for(int i=0;i<n;i++){

&#x20;           for(int j=0;j<n;j++){

&#x20;               if(arr\[j]<min){

&#x20;                   min=arr\[j];

&#x20;               }

&#x20;           }

&#x20;       }

&#x20;       for(int i=0;i<n;i++){

&#x20;           for(int j=0;j<n;j++){

&#x20;               if(arr\[j]>max){

&#x20;                   max=arr\[j];

&#x20;               }

&#x20;           }

&#x20;       }

&#x20;       System.out.print("Maximum:"+max+" Minimum:"+min);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Search element:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.println("Enter size:");

&#x20;       int n=sc.nextInt();

&#x20;       int\[] arr=new int\[n];

&#x20;       System.out.println("Enter array elements:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           arr\[i]=sc.nextInt();

&#x20;       }

&#x20;       System.out.println("Enter the element to be found:");

&#x20;       int key=sc.nextInt();

&#x20;       System.out.println("Array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           System.out.print(arr\[i]+" ");

&#x20;       }

&#x20;       for(int i=0;i<n;i++){

&#x20;           if(arr\[i]==key){

&#x20;               System.out.println("Element found at "+i+" index, position "+(i+1)+" in array.");

&#x20;           }

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

2nd largest number:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc =new Scanner(System.in);

&#x20;       System.out.println("Enter size:");

&#x20;       int n=sc.nextInt();

&#x20;       int\[] arr=new int\[n];

&#x20;       System.out.println("Enter elements:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           arr\[i]=sc.nextInt();

&#x20;       }

&#x20;       System.out.println("Array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           System.out.print(arr\[i]+",");

&#x20;       }

&#x20;       for(int i=0;i<n-1;i++){

&#x20;           for(int j=0;j<n-i-1;j++){

&#x20;               if(arr\[j]>arr\[j+1]){

&#x20;                   int temp=arr\[j];

&#x20;                   arr\[j]=arr\[j+1];

&#x20;                   arr\[j+1]=temp;

&#x20;               }

&#x20;           }

&#x20;       }

&#x20;       System.out.println();

&#x20;       System.out.println("Sorted Array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           System.out.print(arr\[i]+",");

&#x20;       }

&#x20;       System.out.println("2nd largest number is:"+arr\[n-2]);

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Sum, average of elements in array:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc= new Scanner(System.in);

&#x20;       System.out.print("Enter size of array:");

&#x20;       int n=sc.nextInt();

&#x20;       int\[] arr = new int\[n];

&#x20;       double sum=0;

&#x20;       System.out.print("Enter elements of array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           arr\[i]=sc.nextInt();

&#x20;       }

&#x20;       System.out.println("Array:");

&#x20;       for(int i=0;i<n;i++){

&#x20;           System.out.println(arr\[i]);

&#x20;           sum=sum+arr\[i];

&#x20;       }

&#x20;       double avg= (sum/n);

&#x20;       System.out.println("Sum:"+sum+", Average:"+(avg));

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Merge 2 arrays:

public class MergeArrays {

&#x20;   public static void main(String\[] args) {

&#x20;       int\[] a = {1, 2, 3};

&#x20;       int\[] b = {4, 5, 6};

&#x20;       int\[] result = new int\[a.length + b.length];

&#x20;       int index = 0;



&#x20;       // Copy first array

&#x20;       for (int i = 0; i < a.length; i++) {

&#x20;           result\[index++] = a\[i];

&#x20;       }



&#x20;       // Copy second array

&#x20;       for (int i = 0; i < b.length; i++) {

&#x20;           result\[index++] = b\[i];

&#x20;       }



&#x20;       // Print merged array

&#x20;       for (int i = 0; i < result.length; i++) {

&#x20;           System.out.print(result\[i] + " ");

&#x20;       }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Remove duplictaes in array:

public class RemoveDuplicates {

&#x20;   public static void main(String\[] args) {

&#x20;       int\[] arr = {3, 1, 2, 3, 2, 4, 1};

&#x20;       for (int i = 0; i < arr.length; i++) {

&#x20;           int count = 0;

&#x20;           for (int j = 0; j < i; j++) {

&#x20;               if (arr\[i] == arr\[j]) {

&#x20;                   count++;

&#x20;                   break;

&#x20;               }

&#x20;           }

&#x20;           if (count == 0) {

&#x20;               System.out.print(arr\[i] + " ");

&#x20;           }

&#x20;       }

&#x20;   }

}



\------------------------------------------------------------------------------------------------------------------------------------------------------------

palindrome number

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;       System.out.println("Enter number:");

&#x20;       int num=sc.nextInt();

&#x20;       int temp=num;

&#x20;       int rev=0;

&#x20;       while(num!=0){

&#x20;           int rem=num%10;

&#x20;           rev=(rev\*10)+rem;

&#x20;           num=num/10;

&#x20;       }

&#x20;       if(temp==rev){

&#x20;           System.out.println("Palindrome number");

&#x20;       }else{

&#x20;           System.out.println("Not palindrome number");

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Armstrong number:

import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;   System.out.println("Enter number:");

&#x20;   int num=sc.nextInt();

&#x20;   int temp=num;

&#x20;   int arm=0;

&#x20;   while(num>0){

&#x20;       int rem=num%10;

&#x20;       arm=arm+(rem\*rem\*rem);

&#x20;       num=num/10;

&#x20;   }

&#x20;   System.out.println(arm);

&#x20;   if(temp==arm){

&#x20;       System.out.println("Armstrong number");

&#x20;   }

&#x20;   else{

&#x20;       System.out.println("Not armstrong number");

&#x20;   }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Perfect number:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc = new Scanner(System.in);

&#x20;       System.out.println("Enter number:");

&#x20;       int num=sc.nextInt();

&#x20;       int temp=num;

&#x20;       int sum=0;

&#x20;       for(int i=1;i<num;i++){

&#x20;           if(num%i==0){

&#x20;               sum+=i;

&#x20;           }

&#x20;       }

&#x20;       if(temp==sum){

&#x20;           System.out.println("Perfect number");

&#x20;       }

&#x20;       else{

&#x20;           System.out.println("Not perfect number");

&#x20;       }

&#x20;       sc.close();

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Harshad number:
import java.util.Scanner;

class Program{

&#x20;   public static void main(String\[] args){

&#x20;       Scanner sc=new Scanner(System.in);

&#x20;       System.out.println("Enter number:");

&#x20;       int num=sc.nextInt();

&#x20;       int temp=num;

&#x20;       int sum=0;

&#x20;       while(num>0){

&#x20;           int rem=num%10;

&#x20;           sum=sum+rem;

&#x20;           num=num/10;

&#x20;       }

&#x20;       if(temp%sum==0){

&#x20;           System.out.println("Harshad number");

&#x20;       }else{

&#x20;           System.out.println("Not harshad number");

&#x20;       }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Armstrong number: Power of count of digits = number

Harshad number: Sum of digits should divide the number-> 18->1+8=9->18/9=done

Spy number: Sum of digits = Product of digits

Neon number: Sum of digits of square = number

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Prime numbers in range:
class PrimeRange {

&#x20;   public static void main(String\[] args) {

&#x20;       for (int n = 10; n <= 50; n++) {

&#x20;           int count = 0;

&#x20;           for (int i = 1; i <= n; i++) {

&#x20;               if (n % i == 0)

&#x20;                   count++;

&#x20;           }

&#x20;           if (count == 2)

&#x20;               System.out.print(n + " ");

&#x20;       }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

Fibonacci series:

class Fibonacci {

&#x20;   public static void main(String\[] args) {

&#x20;       int a = 0, b = 1;

&#x20;       for (int i = 1; i <= 10; i++) {

&#x20;           System.out.print(a + " ");

&#x20;           int c = a + b;

&#x20;           a = b;

&#x20;           b = c;

&#x20;       }

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------

GCD, LCM:
import java.util.Scanner;

class GcdLcm {

&#x20;   public static void main(String\[] args) {

&#x20;       int a=12, b=18, gcd=1;

&#x20;       for(int i=1;i<=a \&\& i<=b;i++) {

&#x20;           if (a%i==0 \&\& b%i==0)

&#x20;               gcd = i;

&#x20;       }

&#x20;       int lcm=(a\*b)/gcd;

&#x20;       System.out.println("GCD = "+gcd);

&#x20;       System.out.println("LCM = "+lcm);

&#x20;   }

}

\------------------------------------------------------------------------------------------------------------------------------------------------------------















in java, how to get matrix 2x2 :-prompt



Below is TCS‑NQT friendly Java “main logic / syntax” for each matrix operation.

I’m keeping it simple, clean, and exam‑oriented (no extra classes, no advanced tricks).

Assume:

Javaint r = 2, c = 2;int\[]\[] A = new int\[r]\[c];int\[]\[] B = new int\[r]\[c];``Show more lines



✅ 1. Matrix Addition

Logic: Add corresponding elements → C\[i]\[j] = A\[i]\[j] + B\[i]\[j]

Javaint\[]\[] C = new int\[r]\[c];for (int i = 0; i < r; i++) {    for (int j = 0; j < c; j++) {        C\[i]\[j] = A\[i]\[j] + B\[i]\[j];    }}Show more lines



✅ 2. Matrix Subtraction

Logic: C\[i]\[j] = A\[i]\[j] - B\[i]\[j]

Javaint\[]\[] C = new int\[r]\[c];for (int i = 0; i < r; i++) {    for (int j = 0; j < c; j++) {        C\[i]\[j] = A\[i]\[j] - B\[i]\[j];    }}Show more lines



✅ 3. Matrix Multiplication

Condition:

Columns of A == Rows of B

Logic:

C\[i]\[j] += A\[i]\[k] \* B\[k]\[j]

Javaint\[]\[] C = new int\[r]\[c];for (int i = 0; i < r; i++) {    for (int j = 0; j < c; j++) {        C\[i]\[j] = 0;        for (int k = 0; k < c; k++) {            C\[i]\[j] += A\[i]\[k] \* B\[k]\[j];        }    }}Show more lines



✅ 4. Sum of Diagonal Elements

Logic: Primary diagonal → i == j

Javaint sum = 0;for (int i = 0; i < r; i++) {    sum += A\[i]\[i];}Show more lines



✅ 5. Change (Swap) 1st Row with Last Row

Logic: Swap elements row‑wise

Javafor (int j = 0; j < c; j++) {    int temp = A\[0]\[j];    A\[0]\[j] = A\[r - 1]\[j];    A\[r - 1]\[j] = temp;}Show more lines



✅ 6. Sum of 1st Row Elements

Logic: Fix row = 0, loop columns

Javaint sum = 0;for (int j = 0; j < c; j++) {    sum += A\[0]\[j];}Show more lines

