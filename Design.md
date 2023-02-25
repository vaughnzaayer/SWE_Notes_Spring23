## Architecture
- Components and how they talk to each other

## Design
- Individual component operation and composition

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
