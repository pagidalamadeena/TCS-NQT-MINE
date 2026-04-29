**Application Debugging using Visual Studio Debugger**

**NUnit**

**Moq**

**ITIL**

**Windows Service**

\---------------------



\# 1. Introduction to Debugging



&#x20; What is Debugging?



\*   Process of  finding, analyzing, and fixing bugs

\*   Bugs = logical, runtime, or syntax errors



&#x20; Why is Debugging Important?



\*   Ensures correct program behavior

\*   Improves software quality

\*   Reduces production failures

\*   Saves time and cost



&#x20; Why Do We Need Debugging?



\*   Programs rarely work perfectly first time

\*   Helps understand code execution

\*   Identifies root cause of errors



&#x20;



&#x20; Steps Involved in Debugging



\*   Identify the problem

\*   Reproduce the issue

\*   Isolate the faulty code

\*   Fix the bug

\*   Test the solution



&#x20;



&#x20; Debugging Strategies



\*   Divide and conquer

\*   Backtracking

\*   Cause elimination

\*   Logging and tracing



&#x20;



&#x20; Debugging Tools



\*   IDE debuggers (Visual Studio)

\*   Logs

\*   Stack traces

\*   Profilers



&#x20;



&#x20; Debugger vs Debugging



\*    Debugger :

&#x20;   \*   Tool used to debug

\*    Debugging :

&#x20;   \*   Process of fixing errors



&#x20;



&#x20; Debug Mode vs Running Your App



\*   Debug Mode:

&#x20;   \*   Slower

&#x20;   \*   Allows breakpoints and inspection

\*   Run Mode:

&#x20;   \*   Faster

&#x20;   \*   No debugging features



&#x20;



&#x20; When to Use a Debugger



\*   Complex logic issues

\*   Runtime exceptions

\*   Unexpected behavior

\*   Difficult‑to‑trace bugs



&#x20;

😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊

\# 2. Visual Studio Debugger



&#x20; Set a Breakpoint and Start Debugger



\*   Click margin or press  F9

\*   Start debugging with  F5



&#x20;



&#x20; Navigate Code Using Step Commands



\*   Step Into (F11)

\*   Step Over (F10)

\*   Step Out (Shift + F11)



&#x20;



&#x20; Step Over Code



\*   Skips function internals

\*   Executes function as a single step



&#x20;



&#x20; Run to a Point Using Mouse



\*   Right‑click → Run to Cursor

\*   Fast navigation to specific code



&#x20;



&#x20; Advance Out of Current Function



\*   Step Out

\*   Returns to calling method



&#x20;



&#x20; Run to Cursor



\*   Executes code up to selected line

\*   No breakpoint required



&#x20;



&#x20; Edit Code and Continue Debugging



\*   Edit and Continue feature

\*   Modify code during debug session



&#x20;



&#x20; Inspect Variables with Data Tips



\*   Hover over variables

\*   View current values



&#x20;



&#x20; Autos and Locals Windows



\*   Autos → Variables used around current line

\*   Locals → Variables in current scope



&#x20;



&#x20; Set a Watch



\*   Monitor variable values

\*   Add expressions to Watch window



&#x20;



&#x20; Examine the Call Stack



\*   Shows method call hierarchy

\*   Helps trace execution path



&#x20;



&#x20; Inspect an Exception



\*   View exception type and message

\*   Inspect inner exceptions



&#x20;



&#x20; Configure Debugging



\*   Debug settings in project properties

\*   Control symbols, breakpoints, and behavior



&#x20;

😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊

\# 3. Navigating Code Using Visual Studio Debugger



&#x20; Enter Break Mode



\*   Triggered by breakpoint or exception

\*   Pauses execution



&#x20;



&#x20; Code Stepping – Step Into



\*   Enters function calls

\*   Used for deep inspection



&#x20;



&#x20; Step Through and Skip Functions



\*   Step Over avoids entering methods



&#x20;



&#x20; Run to Specific Location



\*   Run to breakpoint

\*   Run to function breakpoint

\*   Run to Click



&#x20;



&#x20; Move the Pointer



\*   Change execution flow

\*   Drag execution pointer to another line

\*   Used cautiously



😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊



\# 4. Automated Testing – Getting Started



&#x20; What is Automated Testing?



\*   Testing using tools/scripts

\*   No manual intervention



&#x20;



&#x20; Benefits of Automated Testing



\*   Faster execution

\*   Repeatable tests

\*   Early bug detection

\*   CI/CD support



&#x20;



&#x20; Types of Tests



\*   Unit Tests

\*   Integration Tests

\*   System Tests

\*   Acceptance Tests



&#x20;



&#x20; Test Pyramid



\*   Unit Tests (base, most)

\*   Integration Tests (middle)

\*   UI/End‑to‑End Tests (top, few)



&#x20;



&#x20; Popular Testing Frameworks



\*   NUnit

\*   xUnit

\*   MSTest



&#x20;



&#x20; Using NUnit in Visual Studio



\*   Install NUnit and NUnit3TestAdapter

\*   Write `\\\\\\\[Test]` methods

\*   Run via Test Explorer



&#x20;



&#x20; What is Test‑Driven Development (TDD)?



\*   Write test before code

\*   Red → Green → Refactor cycle



&#x20;

😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊

\# 5. Fundamentals of Unit Testing



&#x20; Characteristics of Good Unit Tests



\*   Fast

\*   Isolated

\*   Repeatable

\*   Deterministic

\*   Easy to understand



&#x20;



&#x20; What to Test



\*   Business logic

\*   Edge cases

\*   Valid and invalid inputs



&#x20;



&#x20; What Not to Test



\*   Framework code

\*   UI layout

\*   External systems



&#x20;



&#x20; Naming and Organizing Tests



\*   Clear, descriptive names

\*   Group by feature or class



&#x20;



&#x20; Black‑Box Testing



\*   Test functionality without internal knowledge

\*   Focus on inputs and outputs



&#x20;



&#x20; Set Up and Tear Down



\*   Initialize test data

\*   Clean up resources after tests



&#x20;



&#x20; Parameterized Tests



\*   Same test with multiple inputs

\*   Reduces duplication



&#x20;



&#x20; Ignoring Tests



\*   Temporarily disable tests

\*   Used for unstable or incomplete tests



&#x20;



&#x20; Writing Trustworthy Tests



\*   Independent tests

\*   No shared state

\*   Clear assertions



&#x20;

😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊

\# 6. Core Unit Testing Techniques



&#x20; Testing Strings



\*   Equality

\*   Contains

\*   Case sensitivity



&#x20;



&#x20; Testing Arrays and Collections



\*   Count

\*   Order

\*   Expected elements



&#x20;



&#x20; Testing Return Types



\*   Validate type and value

\*   Null vs non‑null checks



&#x20;



&#x20; Testing Void Methods



\*   Verify side effects

\*   Use mocks or state verification



&#x20;



&#x20; Testing Methods that Throw Exceptions



\*   Assert exception type

\*   Assert message if needed



&#x20;



&#x20; Testing Private Methods



\*   Avoid direct testing

\*   Test via public methods



&#x20;



&#x20; Code Coverage



\*   Measures tested code percentage

\*   Helps identify untested logic



&#x20;



\# 7. Breaking External Dependencies



&#x20; Loosely‑Coupled and Testable Code



\*   Minimal dependencies

\*   Easy to mock



&#x20;



&#x20; Refactoring Towards Loose Coupling



\*   Use interfaces

\*   Apply SOLID principles



&#x20;



&#x20; Dependency Injection Methods



\*   Via Method Parameters

\*   Via Properties

\*   Via Constructor (preferred)



&#x20;



&#x20; Dependency Injection Frameworks



\*   Built‑in ASP.NET Core DI

\*   Autofac (external)



&#x20;



&#x20; Mocking Frameworks



\*   Simulate dependencies

\*   Example: Moq



&#x20;



&#x20; Creating Mock Objects Using Moq



\*   Mock interfaces

\*   Define expected behavior



&#x20;



&#x20; State‑Based vs Interaction Testing



\*   State‑Based:

&#x20;   \*   Verify output/state

\*   Interaction:

&#x20;   \*   Verify method calls



&#x20;



&#x20; Testing Interaction Between Objects



\*   Ensure correct collaboration

\*   Verify calls and parameters



&#x20;

😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊

\# 8. ITIL – Getting Started



&#x20; What is ITIL?



\*   IT Infrastructure Library

\*   Best practices for IT service management



&#x20;



&#x20; Why is ITIL Important?



\*   Improves service quality

\*   Aligns IT with business goals



&#x20;



&#x20; What is ITIL 4?



\*   Latest version

\*   Focus on value co‑creation

\*   Agile and DevOps friendly



&#x20;



&#x20; ITIL Service Lifecycle



\*   Service Strategy

\*   Service Design

\*   Service Transition

\*   Service Operation

\*   Continual Improvement



&#x20;



&#x20; Purpose of ITIL Service Operation



\*   Deliver and support services effectively



&#x20;



&#x20; Scope of Service Operation



\*   Daily IT operations

\*   Incident and request handling



&#x20;



&#x20; Business Value of Service Operation



\*   Stability

\*   Reliability

\*   Customer satisfaction



&#x20;



&#x20; Optimization of Service Operation



\*   Long‑Term Incremental Improvement

\*   Short‑Term Ongoing Improvement



&#x20;



\# 9. Functions of ITIL Service Operation



&#x20; Service Desk



\*   Single point of contact

\*   Handles incidents and requests



&#x20;



&#x20; Technical Management



\*   Provides technical expertise

\*   Maintains infrastructure



&#x20;



&#x20; IT Operations Management



\*   Manages daily operations

\*   Job scheduling and monitoring



&#x20;



&#x20; Application Management



\*   Supports applications

\*   Ensures application availability



&#x20;



\# 10. Processes Under Service Operation



&#x20; Event Management



\*   Monitors events

\*   Detects issues early



&#x20;



&#x20; Incident Management



\*   Restores service quickly

\*   Minimizes impact



&#x20;



&#x20; Problem Management



\*   Finds root cause

\*   Prevents recurrence



&#x20;



&#x20; Request Fulfilment



\*   Handles service requests

\*   Access, information, software



&#x20;



&#x20; Access Management



\*   Controls user access

\*   Ensures security



&#x20;

😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊😊

\# 11. Windows Services – Introduction



&#x20; What is a Windows Service?



\*   Background application

\*   Runs without user interaction



&#x20;



&#x20; Why We Need Windows Services?



\*   Long‑running tasks

\*   Continuous background processing



&#x20;



&#x20; Windows Service Control Manager (SCM)



\*   Manages services

\*   Starts, stops, and monitors services



&#x20;



&#x20; Windows Services vs Regular Applications



\*   No UI

\*   Starts automatically

\*   Runs in background



&#x20;



&#x20; Examples of Windows Services



\*   Print Spooler

\*   Windows Update

\*   SQL Server Service



&#x20;



\# 12. Developing and Managing a Windows Service



&#x20; Installing the Windows Service



\*   Register service with SCM

\*   Use installer or command line



&#x20;



&#x20; Starting the Windows Service



\*   Via Services console

\*   Programmatically

\*   Command line



&#x20;



&#x20; Stopping the Windows Service



\*   Services console

\*   Command line

\*   Programmatic stop

