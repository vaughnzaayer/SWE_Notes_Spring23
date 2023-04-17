## Architecture
- Components and how they talk to each other
	- Components and their interactions are defined

- Components broken down into two main parts:
	- Functionality
	- Data

- How is control managed?

### Examples: Architecture
- [[#Client-Server Architecture:|Client-Server]]
	- Crud
- Peer-2-Peer
- Pipe and Filter
- Layered
- Object-Oriented (Family)
- Event-Based

### Client-Server Architecture
- Clients want to use a system
- Servers that manage system functionality of data & provide responses
[[Drawing 2023-02-27 10.10.31.excalidraw|Server/Client Diagram]]
![[Drawing 2023-02-27 10.10.31.excalidraw.svg]]

### Client-Server-Broker Architecture
- Same as [[#Client-Server Architecture]], except has an intermediary "broker"
- Broker will reroute client/server relationships to manage things like load balancing, etc.
- Brokers can become bottlenecks, and can overall degrade performance

### Pipe and Filter
- Only need to know input/output formats
- Implemented, runs in parallel
- Modularity of the filters
- Unix/Linux cmd line, compilers, signal processing, etc.
![[Drawing 2023-03-01 10.11.45.excalidraw.svg]]

### Object-Oriented
- Expose external variables & methods
- *Encapsulate* internal variables & methods
- Objects must know about other objects to interact with

![[Drawing 2023-03-01 10.20.26.excalidraw.svg]]

### Event-Based
- Announcers don't worry about how events will be handled
- Modularity of agents
- Controlling ordering is difficult
- Used in debugging, database management, (G)UIs

![[Drawing 2023-03-01 10.33.10.excalidraw.svg]]

### Layered Systems
- Closed Layered: Each layer can only talk to adjacent layers
	- Minimizes dependencies
	- Reducing impact of change
- Open Layered: Layers can use the services of lower layers
	- More compact code
	- Breaks some encapsulation
- Good for abstraction + encapsulation
- Easy to add, remove layers, including partitioning of layers
- Used in OS (kernel is lowest, GUIs is highest for example), communication protocols (Internet)

![[Drawing 2023-03-01 10.37.39.excalidraw.svg]]

### Repositories
- Central shared data space called "blackboard"
- Issue of bottlenecking occurs

#### Model-view controller


### Community within Architectures
- *Coupling:* inter-component interactions, how much interaction is there between different components
	- Architecture should have *less* coupling
- *Cohesion:* intra-component interactions, how much interaction between the same component
	- Architecture should have *high* coherence


## Design
- Individual component operation and composition

### Principles
- *Motivation:* Each concept should have a purpose
- *Coherence:* Each concept should have *at most* one purpose
- *Fulfillment:* Each purpose should motivate at least one concept
- *Non-Division:* Each purpose should motivate at most one concept
- *Decoupling:* Concepts should not interfere with other fulfillment of purpose


## How to Model Data
*At an abstract level* 

*Entities*
- What are the types of data in the system?
	- NOT language types (int, float, etc.)

*Relationships*
- How do entities interact?

*Attributes*
- Relevant elements of entities

### Example: Course Registration
#### Entities
- Students
- Course
- Time
- Instructor

#### Relationships
- Students enroll in courses
- Courses have instructors
- Courses have times
- Courses have other courses as prerequisites
- Students have course history


## Entity-Relationship Diagrams
Models how each entity interacts with one another

### Breakdown
- Entities are **rectangles**
- Attributes are **circles**
	- **Underlined** attributes are critical and identifiers for an entity
- Relationships are **diamonds**


## Design Principles

### Information Hiding (Encapsulation)
- Interface vs Implementation
	- What our components do vs how our components do this
- Interface should be publicly visible
- Implementation should not be publicly visible 
- Important for *refactoring* 
- Allows changes to code to affect only components that rely on implementation

### Polymorphism
- When an operation's behavior can change based on parameters
- 3 Types:
	- Ad-hoc polymorphism 
		- (A + B)
		- Integer arith.
		- Calling object methods
		- Concatenating strings 
	- Subtype Polymorphism 
		- (obj.toString();)
	- Parametric Polymorphism
		- Templates in C++ to create type-specific objects


### Open/Closed Principle
- Components should be open for *extension* and closed for *modification*

### Avoid the Diamond of Death
- Avoid having classes inherit from multiple parent classes

### Composition over Inheritance
- has-a > is-a

### Listcov Substitution Principle
- Any property of a parent class should be true for all subclasses


