Definition
Decouple an abstraction from its implementation so that the two can vary independently.



Bridge: when and where you would use it

The Bridge pattern is used for decoupling an abstraction from its implementation so that the two can vary independently. Bridge is a high-level architectural patterns
and its main goal is through abstraction to help .NET developers write better code. A Bridge pattern is created by moving a set of abstract operations to an interface
so that both the client and the service can vary independently. The abstraction decouples the client, the interface, and the implementation.

A classic example of the Bridge pattern is when coding against device drivers. A driver is an object that independently operates a computer system or external hardware
device. It is important to realize that the client application is the abstraction. Interestingly enough, each driver instance is also an implementation of the Adapter
pattern. The overall system, the application together with the drivers, represents an instance of a Bridge.


Real-world sample code
The real-world code demonstrates the Bridge pattern in which a BusinessObject abstraction is decoupled from the implementation in DataObject. The DataObject
implementations can evolve dynamically without changing any clients.

Code in project: DoFactory.GangOfFour.Bridge.RealWorld
.NET optimized sample code
The .NET optimized code demonstrates the same code as above but uses more modern, built-in .NET features. The DataObject abstract class has been replaced
by an interface because DataObject contains no implementation code. Furthermore, to increase type-safety the customer list was implemented as a generic List
of strings: List<string> in C# and List(Of String) in VB.

