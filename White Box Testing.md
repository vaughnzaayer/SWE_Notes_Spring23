- Look at the implementation of our software, and test each feature (to as great of an extent as possible)

## Coverage Testing
- Focuses on the code itself

### FSM Testing
- Cover all vertices
- Cover all edges
- Cover all paths
- Cover invalid transitions


## State Testing
- Focuses on a representation of the code's decision making

### Control Flow Graph
- Construct node-based graphs based on the code's control flow (for example, if/else statements)
- Thorough but expensive
- Effectively testing every line of code (*Statement Coverage*)
- We could also test every diverging branch in the graph (*Decision Coverage*)
- Check every boolean (*Condition Coverage*)

#### Modified Condition/Decision Coverage
- Each decision has both values (0/1) tested
- Each condition has both values (0/1) tested
- Every condition is shown to independently effect its decision


## Mutation Testing
- Making incremental changes to the existing software
- Generates test cases and checks test coverage


## Types of Testing

### Unit Tests
- Focus on individual components
- Horizontal Testing
	- Combine things one level at a time
- Vertical Testing
	- Combine things one functionality at a time

### Integration Tests
- Focus on combined components

### System Tests
- Type of Integration Test, *everything* is integrated
- Testing end-to-end functionality of a system

### Acceptance Tests
- Systems test w/ clients