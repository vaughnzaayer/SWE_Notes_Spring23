
## Methodologies For Designing Software

### Ad-Hoc
- Latin -> "To this"
- How you design Software if you're not thinking about the process

#### Steps
- Have ideas
- Write code
- See if it works
- Debug

#### Pros
- Saves time if it actually works!
- Good for small, quick prototypes
- *Low Overhead*

#### Cons
- Wasted time if it doesn't work
- Not scalable
- Not compatible 
- Less extendable/modifable
- **Teamwork is hard**
- Testing is going to be worse


### Formalized

#### Steps Shared Across Methodologies
**Write Documentation Throughout Process**
1) *Requirements*
	- What should software do?
	- [[Requirements]]
2) *Design*
	- How should the software do it?
	- What language? Existing software? etc.
3) *Implementation*
	- Write the code!
	- Testing is in part written here
4) *Validation*
	- Run the tests
	- Evaluate requirements
	- Connect with user
5) *Release*
	- Make the code/software available
6) *Maintenance*
	- Make sure to update the software to keep it secure and modern
	- Bug fixes!


#### Waterfall Design Methodology

##### Process (Finish ALL of Each Step)
*See:* [[Software Design Methodologies#Steps Shared Across Methodologies |Common Steps]]
1) Step 1
2) Step 2
3) etc.

- What happens when something isn't perfect? Go back a step

##### Pros
- Simple on paper *and only* on paper
- Little overhead! (as long you don't mess anything up)
- Probably good for smaller projects

##### Cons
- Not Ad Hoc
- If you need to backtrack, there's no infrastructure for it
	- So it's wildly inefficient
- Doesn't scale well with larger teams and projects
- Timeline is murky


#### Spiral Model
Developed by Barry Boehm
- The "spiral" on the graph represents the path of development
- Each step is passed through several times

##### Process
Each step matches to a quadrant on the 2D graph
1) Determine objectives
	- *Requirements*
2) Identify and Resolve Risks
	- Emphasis on *Risk Management*
	- Risk includes things like monetary investment, software failures
		- "What can go wrong?"
	- Focus on mitigation and alternatives
3) Development + Tests
	- *Implementation* & *Validation*
	- Tests are designed and run here
4) Plan the next Iteration
	- Emphasis on *learning*
		- What went well?
		- What went poorly?
		- What to keep and change?
	- Additional overhead compared to [[Software Design Methodologies#Waterfall Design Methodology |The Waterfall Model]]

##### Pros
- No need to completely backtrack
	- Just need to wait for the next iteration
- Guaranteed progress, clear prototypes

##### Cons
- Bit more overhead in step 4
- Forced synchronization
- Overhead in testing


#### Prototyping
A prototype is an implementation that is not designed to be final, but to be a proof of concept for important features

- Emphasis on *small scale*
- Includes the [[Software Design Methodologies#Spiral Model |Spiral Model]]
- Sometimes considered a design model
- Issue of fidelity:
	- What features to capture? (*Breadth*)
	- How fleshed out are they? (*Depth*)

##### Paper Prototyping
- Particular type of prototyping focused on *user interaction* without code
- A human pretends to be the software, essentially
- Allows you to see if the user interactions are doing what you expect