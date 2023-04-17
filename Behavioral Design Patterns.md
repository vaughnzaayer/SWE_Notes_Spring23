*How objects perform their functionality*

## Strategy Pattern
- [[UML Diagrams|UML]] pattern is the same as the [[#Bridge Pattern]], except it describes composition of methods instead of data


## Iterator Pattern
- Lets the user access each and every element in a data structure
- *Iterator* objects have the following functionalities (usually):
	- Method to go to the "next" object
	- Method that tells you if there are more objects in the structure
- Iterators are compatible between different types of data structures
	- List Iterator, Map Iterator, Set Iterator, etc.
- *Collection* objects can return an iterator for each of its data types


## Observer Pattern
- Track the interested (*Subscribers) and uninterested objects to receive events/notifications from another object (*Publisher*)
- Publisher class
	- has collection of subscribers
	- has notifySubscribers() method
	- has addSubscriber() method
	- has removeSubscriber() method
- Subscriber class
	- has respond(event) method


## Visitor Pattern
Huh?


## State Pattern
- "State" component of a class 
	- Contains methods for the class
	- Ex. Publish, Notify Collaborators, etc.
- State has different types of subclasses which decide the object's functionality