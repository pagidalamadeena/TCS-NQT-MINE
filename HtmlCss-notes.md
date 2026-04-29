**Html**: Standard language used to create and design the structure of webpages.



Structure: doctype, html tag,(head, body, footer) section

&#x20;

Tag: word in <,>.



Element: Start tag, content, end tag.

<p> Hi, Welcome to Html. </p>



Attribute: Extra details about the tag, will be included in opening tag.



Class: group of elements, used to apply same styling

id: unique identifier for element



Head Section: Contains-> metadata, title, styles, and scripts\[Not displayed on webpage]

\* title defines the name of the webpage shown in the browser’s tab.

\* Metadata is information about the webpage, such as author and description, placed inside the <head> section.



Body Section: Contains all the visible content of webpage, such as links, text, images.



Footer Section:



Basic Tags of Html:

1\. <p></p>

2\. <br>

3\. <h1>....<h6>

4\. <a href="">Link</a>

5\. <li></li>, types->ol,ul

6\. <div> is a block‑level container used to group HTML elements.

7\. <img src="" alt="">

8\. <span> used to inline style block of content.

9\. <form> user input form

10\. <input type="text" placeholder="Enter name">

11\. <script> to add javascript to webpage

12\. <table>, <th> table head, <tr> table row, <td> table data



**Sample** **code**:

<!DOCTYPE html>

<html>

<head>

&#x20; <title>CSS Selectors Demo</title>

&#x20; <link rel="stylesheet" href="style.css">

</head>

<body>



&#x20; <h1 id="mainTitle">CSS Selectors</h1>



&#x20; <p>This is a normal paragraph.</p>

&#x20; <p class="highlight">This is a highlighted paragraph.</p>



&#x20; <div class="box">

&#x20;   <p>Paragraph inside div</p>

&#x20;   <span>Span inside div</span>

&#x20; </div>



&#x20; <input type="text" placeholder="Enter your name">



</body>

</html>

\-------------------------------------------------------------------------------------------------------

**CSS**: Cascading Style Sheet, used to style the webpages



Selector: select the content that we want to apply styling

\* Id selector(#)

\* Class selector(.)

\* Element selector

\* Universal selector(\*)



Property: type of style, color,bg-color.,etc

Value: such as red,20px.,etc

Declaration: combines property \& value, color : "red"



Rule: CSS block containing a selector and declaration block.

p{

color : "red";

}



Types of CSS: Inline, Internal, External



Box Model: The structure of every HTML element consisting of:

content → padding → border → margin



Flexbox: layout system used to align elements horizontally or vertically



Grid: A two‑dimensional layout system used to create complex page layouts.

Some of CSS styles:

1\. text color

2\. background color

3\. margin

4\. padding

5\. position

6\. animation

7\. transition

8\. Z index.,etc





Sample code:
p {

&#x20; color: blue;

}

\#mainTitle {  // Applies only to the element with id="mainTitle".

&#x20; color: darkgreen;

&#x20; text-align: center;

}

.highlight { //Applies to all elements with class="highlight".

&#x20; background-color: yellow;

&#x20; font-weight: bold;

}

h1, p { //Group selector

&#x20; font-family: Arial, sans-serif;

}

div p { //Selects elements inside another element-Only <p> inside <div> turns red.

&#x20; color: red;

}

input\[type="text"] { //Selects elements with a specific attribute-Styles only text input boxes.

&#x20; border: 2px solid blue;

&#x20; padding: 5px;

}

\* {

&#x20; margin: 0;

}





Selector               Example           Meaning

Element                  p              All <p> elements

ID                       #id            NameOne specific element

Class                   .className      Group of elements

Group                   h1, p           Multiple elements

Descendant              div p           <p> inside <div>

Universal                \*              All elements

Attribute          input\[type="text"]   Specific attribute



\--------------------------------------------------------------------------------------------------------------

**CSHTML:** is a Razor view file used in ASP.NET / ASP.NET Core MVC applications.

Key points:

* Combines HTML + C#
* Used for dynamic web pages
* Runs on the server
* Requires ASP.NET framework



Feature                HTML                  CSHTML

File extension         .html                 .cshtml

Type                  Markup language        Razor view (HTML + C#)

Server-side code      ❌ No                  ✅ Yes

Dynamic content       ❌ No                  ✅ Yes

Framework needed      ❌ No                  ✅ ASP.NET

Execution            Browser               Server → Browser

