# mid-exam-prparation
mid-exam-prparation
Window programming pre-mid Exam Mocup Answers
Group Members:                                    ID
1.Hareg Bekele          UUR01373/16
2.Melat Tesfaye         UUR00922/16
3.Kawser Awel           UUR00409/16
Part 1: Software Devlopment( Chapter 1)
Question 1 (B): Food-Delivery Mobile App for a Startup
Recommended SDLC Model: Agile/Scrum
Agile/Scrum is the best model for developing a food-delivery mobile application because the startup operates in a rapidly changing market.
Reasons:
1.Changing Requirements: Customer needs and market demands can change frequently.
2.Fast Development: Agile allows developers to release the application quickly.
3.Customer Feedback: Customers can give feedback, and developers can improve the application.
3.Flexibility: Developers can easily add new features or modify existing ones.
4.Continuous Testing: Each development iteration is tested to identify and fix errors.
4.Testing: Testing is performed after each sprint to ensure the application works correctly and satisfies customer requirements.
5.Conclusion: Agile/Scrum is suitable because it supports flexibility, fast delivery, continuous testing, and customer satisfaction.
Question 2: The Hidden Trade-offs of Rapid Application Development (RAD)
RAD focuses on fast software development by using rapid prototyping instead of extensive upfront planning. However, skipping proper planning can create scalability and reliability problems in the future.
1. Poor Planning: Without proper planning, developers may create a weak system structure that becomes difficult to maintain.
2. Architectural Debt: Developers may choose quick solutions instead of strong designs. Later, fixing these problems becomes expensive and difficult.
3. Scalability Problems: The application may work well with a small number of users but fail when many users access it at the same time.
4. Reliability Problems: Limited planning and testing can cause errors, system failures, and unexpected problems.
5. High User Availability Demands: The system may not be properly designed to support users who need continuous access.
6. Lack of Deep Risk Analysis: Developers may fail to identify important technical risks before they become serious problems.
Q3. Balancing Software Development Principles
Yes. Following DRY and Separation of Concerns too much can violate KISS and YAGNI.
For example, creating many unnecessary classes and interfaces for a simple calculator makes the program complicated.
DRY: Avoid code repetition.
KISS: Keep code simple.
YAGNI: Avoid unnecessary features.
Separation of Concerns: Divide responsibilities.
Q4. The Economics of Testing and Code Quality
Fixing errors early is cheaper because problems are easier to identify and correct before deployment.
Three practices help reduce errors:
1.TDD: Write tests before writing code.
2.Continuous Integration: Regularly combine and test code.
3.Peer Code Review: Ask other developers to check your code.
Q5. MSIL, JIT, and Platform Independence
.NET follows these steps:
1.C# code is compiled into MSIL.
2.JIT converts MSIL into native machine code
3.CLR manages program execution.
Traditional .NET Framework applications depend on Windows because they use Windows-specific CLR and libraries.
Mono: Mono is a cross-platform implementation that allows .NET applications to run on Windows, Linux, and macOS.

Q6. Managed vs. Unmanaged Code & Language Interoperability
Managed Code:
Runs under CLR.
Uses automatic memory management.
Unmanaged Code:
Runs outside CLR management.
Often requires manual memory management.
Example: Traditional C/C++.
Language Interoperability:
It means different programming languages, such as C#, VB.NET, and F#, can work together in the .NET environment
7. Solving "DLL Hell"
The problem: before .NET, applications shared DLLs. When a new application was installed, it could replace a shared DLL with a different version, and the old applications that needed the old version stopped working.
How .NET solves it:
Assemblies:  the unit of deployment. An application can keep its own private assembly in its own folder, so no other app can overwrite it.
Manifest and metadata:  every assembly has a manifest that lists its name, its version, and the versions of the other assemblies it needs. The CLR uses it to load the correct versions.
Strong names: a strong name (name, version, culture and a public key) gives the assembly a unique identity, so two different assemblies can't be mixed up.
GAC (Global Assembly Cache): a place to keep shared assemblies. Many versions of the same assembly can live there side by side, and each application uses the version it needs.
Why namespace and assembly are not the same thing:
A namespace is a logical grouping of classes (for example System.Windows.Forms). It helps us organize code and avoid name conflicts.
An assembly is a physical grouping. It is the actual .exe or .dll file we deploy.
One assembly can have many namespaces, and one namespace can be in many assemblies.
Q8. Abstraction in Data Access: ADO.NET vs. Entity Framework & LINQ
It asks why manually working with database connections and DataSets is more difficult than using Entity Framework and LINQ.
ADO.NET requires developers to:
Open and close database connections manually.
Write SQL queries manually.
Convert database results into objects.
Handle errors and data manually.
Entity Framework makes database access easier by automatically converting database tables into .NET objects.
LINQ allows developers to write queries using a common syntax to work with SQL databases, XML, and collections.
Advantages of Entity Framework and LINQ:
1.Less code.
2.Easier database management.
3.Reduced manual errors.
4.Improved readability.
5.Faster development.
Trade-off: Entity Framework provides convenience, but can introduce performance overhead and less direct control compared with manual SQL.
.Q9. Under the Hood of Event-Driven Programming
A console application runs instructions sequentially, but a Windows Forms application waits for user actions.
In Windows Forms, event-driven programming works as follows:
1.Main(): Starts the application.
2.Main Loop: The application waits for user actions.
3.Event Listener: Monitors user actions such as button clicks.
4.Event: A button click generates an event.
5.Event Handler: The associated method executes the code.
6.Delegate: Connects the event to its handler.
7.Lambda Expression: Can provide a short event-handling method.


