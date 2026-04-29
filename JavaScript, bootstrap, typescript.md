JavaScript, bootstrap, typescript:



**JavaScript** **Notes:**

⭐ 1. Fundamentals



JavaScript is used to make web pages interactive.

✅ Variables → let, const, var

✅ Data Types → string, number, boolean, null, undefined, object, array



⭐ 2. Operators

➕ Arithmetic → + - \* / % ++ --

🔁 Assignment → = += -= \*=

🔍 Comparison → == === != !== > < >= <=

✅ Logical → \&\& || !

🔗 String → "Hello" + "World"



⭐ 3. Control Flow

✅ if / else

✅ switch

✅ Loops:

for

while

do...while

for...of (arrays)

for...in (objects)



⭐ 4. Objects

Store data in key–value pairs.

const person = {  name: "John",  age: 30};



⭐ 5. Arrays

List-like structures.

let fruits = \["apple", "banana"];



Useful methods → push, pop, map, filter, forEach



⭐ 6. Functions

Reusable blocks of code.

function add(a, b) { return a + b; }

Arrow function:

const add = (a, b) => a + b;



⭐ 7. DOM (Document Object Model)

DOM is a programming interface that represents a web page as a tree of objects, so JavaScript can access, change, add, or remove HTML elements.

✅ In simple words:

DOM = HTML page + JavaScript control



2\. Why do we need DOM?

Without DOM:

HTML would be static

No dynamic updates



With DOM:

Change text

Change styles

Handle button clicks

Add/remove elements dynamically





3\. How DOM Works

Browser loads HTML

Browser converts HTML into a tree structure

JavaScript interacts with this tree using DOM methods



Example HTML

HTML<body>

<h1 id="title">Hello</h1>  

<p>This is a paragraph</p></body>



DOM Tree (Simple view)

Document

&#x20;└── html

&#x20;    └── body

&#x20;        ├── h1

&#x20;        └── p



Each tag becomes an object (node).



4\. Main Parts of DOM

* Document → whole web page
* Elements → HTML tags (h1, p, div)
* Attributes → id, class, src
* Text → content inside tags





5\. Accessing Elements (Very Important)

By ID:-

JavaScriptdocument.getElementById("title");

By Class:-

JavaScriptdocument.getElementsByClassName("box");

By Tag:-

JavaScriptdocument.getElementsByTagName("p");



JavaScript can change HTML/CSS dynamically.

✅ Events:

button.addEventListener("click", () => {});



✅ Button click example:
<button onclick="changeText()">Click Me</button>

\----------------------------------------------------------------------------------------------------------------------------------------------------------

**Bootstrap** 5 Notes:

⭐ 1.What is Bootstrap?

Bootstrap is a free front-end framework that helps you design websites quickly and easily.

✅ It is mainly used for:

Styling web pages

Creating responsive layouts

Making pages look professional without writing much CSS



👉 In short:

Bootstrap = Ready‑made CSS + JavaScript tools



Why Bootstrap Was Created

Writing CSS from scratch:

Takes time

Needs careful alignment

Breaks on different screen sizes



Bootstrap solves this by providing:

Pre-written CSS classes

Built-in layouts

Mobile-friendly designs



Bootstrap includes:

CSS – for styling

JavaScript – for interactions

Components – buttons, cards, navbars, etc.

Grid system – for page layout



\### ⭐ 2. Layout \& Grid System



| Concept        | Explanation (Simple)                    | Example Meaning         |

| -------------- | --------------------------------------- | ----------------------- |

| 12‑column grid | Screen is divided into 12 equal columns | Layout becomes flexible |

| `row`          | Creates a horizontal row                | Holds columns           |

| `col-6`        | Takes 6 out of 12 columns               | Half of the screen      |

| `col-12`       | Takes all 12 columns                    | Full width              |

| Breakpoints    | Change layout for screen sizes          | sm, md, lg, xl, xxl     |



\*\*Example Explanation\*\*\\

`col-6 + col-6 = 12` → two equal columns



sm-small (mobile)

md- medium (tablets)

lg- large screen (laptops)

xl- extra large

xxl- extra largest

\*\*\*



\### ⭐ 3. Essential Bootstrap Components



| Component | Purpose             | Example Class     |

| --------- | ------------------- | ----------------- |

| Button    | Click actions       | `btn btn-primary` |

| Card      | Show content in box | Card layout       |

| Navbar    | Top navigation bar  | Menu/Header       |

| Modal     | Popup window        | Login/Alert       |



\*\*\*



\### ⭐ 4. Utilities \& Helper Classes



| Category | Class         | What It Does        |

| -------- | ------------- | ------------------- |

| Spacing  | `m-3`         | Adds margin         |

| Spacing  | `p-2`         | Adds padding        |

| Text     | `text-center` | Centers text        |

| Text     | `fw-bold`     | Makes text bold     |

| Display  | `d-flex`      | Enables flex layout |

| Display  | `d-none`      | Hides element       |

| Colors   | `text-danger` | Red text            |

| Colors   | `bg-dark`     | Dark background     |



✅ Small classes that save writing CSS



\*\*\*



\### ⭐ 5. Responsive Design



| Class             | Meaning                               |

| ----------------- | ------------------------------------- |

| `col-12`          | Full width on small screens           |

| `col-md-6`        | Half width on medium \& larger screens |

| Responsive design | Layout changes based on device size   |



\*\*Example Explanation\*\*

\*   Mobile → Full width

\*   Tablet \& Laptop → Half width



\*\*\*



\## ✅ One‑Look Revision Summary



| Topic             | Key Idea              |

| ----------------- | --------------------- |

| Grid system       | 12‑column layout      |

| Components        | Ready‑made UI parts   |

| Utilities         | Quick styling helpers |

| Responsive design | Fits all screens      |





\-----------------------------------------------------------------------------------------------------------------------------------------------------------

🟦 TypeScript Notes

⭐ 1. Introduction

TypeScript = JavaScript + Type Safety

Helps avoid runtime errors.





⭐ 2. Basic Types

let isActive: boolean = true;

let age: number = 20;

let name: string = "John";



⭐ 3. Type Annotations \& Inference



Type Annotation (Explicit): You manually specify the type.

let count: number = 10;



Type Inference (Automatic/Inferenece/Implicit): TypeScript detects the type automatically.

let count = 10; // inferred as number(int)







⭐ 4. Functions

function add(a: number, b: number): number {  return a + b;}

Optional parameters:

function greet(name?: string) {}



⭐ 5. Interfaces \& Object Types

An interface defines the structure of an object. Ensures object follows the defined format

interface Person {

&#x20; name: string;

&#x20; age: number;

}



let user: Person = {

&#x20; name: "John",

&#x20; age: 25

};



⭐ 6. Classes \& Access Modifiers

class Car {

&#x20; private model: string;

&#x20; public year: number;



&#x20; constructor(model: string, year: number) {

&#x20;   this.model = model;

&#x20;   this.year = year;

&#x20; }

}



✅ Access modifiers: Used for data hiding and security



Modifier               Meaning

public           Accessible everywhere

private          Accessible only inside the class

protected        Accessible in class \& subclasses





⭐ 7. Union \& Literal Types



Union type: Allow a variable to have multiple types. Can store number/string.

let id: number | string;



Literal type: Allow only specific values.

let direction: "left" | "right";



Topic                  Key Meaning

TypeScript        JavaScript with type safety

Basic types       Boolean, number, string

Annotation        Explicit type

Inference         Automatic type detection

Functions         Typed inputs \& outputs

Interface         Object structure

Class             Blueprint of objects

Access modifiers  Control visibility

Union type        Multiple data types

Literal type      Fixed values only

