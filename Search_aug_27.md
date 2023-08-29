### Introduction:
We will cover various techniques that are foundations of AI. Anything that involves a bit of intelligence for the machine to perform tasks can be termed as AI. We will see about these following techniques
- search
- knowledge representation
- uncertainity
- optimization
- machine learning- neural networks
- Language - Natural language processing.

#### Search
Let's say we have got a problematic situation. To 'find' solution for that situation we call 'search'
for example - a maze game or slide the number tile game.
###### Terminologies:
- Agent: The agent percieves and performs actions in an environment.
- State: A particular configuration of environment, an instance.
- Initial state: State from which agent begins.
- Actions: An agent performs actions to bring change in the state.
- Transition model: It is the result of action performed by the agent on the state
- State space: A set of all the achievable states in the environment.
- goal test: A test performed to check if the current state is our goal.
- Path cost: We define a cost for every action the agent performs, and we try to minimize it.
- Optimal solution: It is the best solution to the given problem, path cost is lowest.
- node: This is a datastructure which stores
   - a state
   - data about parent state
   - actions it can perform
- Stack: It is a data structure where the first thing that comes goes last

##### Approach:
- Start with a frontier that contains the inital state
- Repeat:
   - If the frontier is empty, then no solution
   - Remove a node from the frontier
   - If node contains goal state, return the solution
   - Expand node, add resulting nodes to the frontier
**Disadvantage of this approach**
If we can reach parent node from the considered node, we may essentially move in an infinite loop
**Solution of this problem is to keep a track of already explored node, and we should not add them to frontier in future explorations.**

