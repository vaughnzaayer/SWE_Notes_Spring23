
## Composite Design Patterns
- Object types that are combinations of other object types

### Adapter Pattern
- Same functionality, different interface
- Adds additional functionality while using the same interface

### Proxy Pattern
- Same functionality, same interface
- Communication, routing, load balancing

### Decorator Pattern
- Different functionality, same interface


## Facade Pattern
- Presenting a different face than what's actually "behind"
- Provides a "Facade", or simplified interface, for external users to interface with 


## Fly Weight Pattern
- Aimed at reducing weight of implementations
- Complicated data sound be shared when possible, usually uses pointers, references


## Bridge Pattern
- When making a new instance of a type/class, another type/class can be used to specify and create new methods within the new instance
	- Ex. *Triangle MonitorTriangle = new Triangle(new MonitorDisplay())* vs *Triangle VRTriangle = new Triangle(new VRDisplay())*
- Specifically, a class is composed of some other class/method class


