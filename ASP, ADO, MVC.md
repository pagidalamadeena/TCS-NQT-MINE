ASP, ADO, MVC



✅ 1. ASP.NET: (Active Server Pages) ASP.NET is a web application framework developed by Microsoft for building dynamic web applications, web APIs, and websites. Examples: forms, login, data-driven webpages

✅ Key Points (Interview Level):-

Built on the .NET Framework / .NET Core.

Supports multiple languages like C# and VB.NET.

Provides server‑side web development.

Rich toolbox in Visual Studio.



Offers features like:

State Management: (ViewState, Session, Cookies, Application)

Server Controls: (GridView, TextBox, Button)

Security: (Forms authentication, Windows authentication)





✅ Types of ASP.NET Applications:-

Web Forms (event-driven model)

MVC (model-view-controller pattern)

Web API (RESTful services)

ASP.NET Core (cross‑platform)



✅ Typical Interview Question

Q: What is the difference between ASP.NET Web Forms and ASP.NET MVC?

✅ Web Forms – ViewState, page life cycle, server controls.

✅ MVC – Lightweight, testable, clear separation of concerns.



✅ 2. ADO.NET: (ActiveX Data Objects) ADO.NET is a data access technology used to interact with databases like SQL Server, Oracle, etc.

✅ Why ADO.NET?

It helps:

Connect to a database

Execute commands

Retrieve results

Update data



✅ Core Components:-

**Component**      -      **Purpose**

Connection            Connects to the database

Command               SQL queries / stored procedures

DataReader            Fast, forward‑only data

DataAdapter           Fills DataSet using select query

DataSet               In‑memory database (disconnected)



✅ Connection Models



Connected Architecture:-

Uses DataReader

Faster, less memory usage





Disconnected Architecture:-

Uses DataSet, DataTable

Works offline, heavy







✅ Typical Interview Question

Q: Difference between DataSet and DataReader?

✅ DataReader – Connected, fast, forward‑only.

✅ DataSet – Disconnected, can store multiple tables, slower.



✅ 3. MVC (Model‑View‑Controller)

MVC is a software architectural pattern used to separate an application into three parts:

✅ Components



Model:

Business logic

Data and validation



View:

UI / HTML pages



Controller:

Handles requests

Communicates between Model \& View





✅ Advantages of MVC

Clear separation of concerns

Easy to maintain and test

Supports TDD (Test‑Driven Development)

No ViewState → lightweight and fast

SEO‑friendly URLs



✅ Request Flow

Browser → Controller → Model → View → Browser

&#x20;

✅ Typical Interview Question

Q: What is Routing in MVC?

✅ Routing maps URL requests to specific controllers and actions.



✅ 4. ASP (Classic ASP)

ASP (Active Server Pages) is the older, pre‑.NET Microsoft web technology.

✅ Key Points



Scripting language: VBScript / JavaScript

No code-behind separation

Limited debugging

Not strongly typed

Not object‑oriented

Replaced by ASP.NET



Q: Difference between ASP and ASP.NET?

✅ ASP – Scripting, old, interpreted.

✅ ASP.NET – Compiled, object‑oriented, supports C#, faster, secure.





Controllers: Handle incoming requests, coordinate logic, and return responses.

Models: Represent application data and business rules.

Views: Display data to the user as UI/output.

Services: Contain business logic and reusable operations.

Repositories: Manage data access and database operations.

DTOs (Data Transfer Objects): Transfer data between layers without business logic.

Interfaces: Define contracts for classes to ensure consistency and loose coupling.

Helpers: Provide common utility functions used across the project.

