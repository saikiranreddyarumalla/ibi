# What are Higher-Order Components (HOC) in React and how do they work?
## ANS:
Higher-Order Components (HOC) in React are functions that take a component as input and return a new component with added functionality. They allow reusing and enhancing component behavior, such as managing state, handling data fetching, or providing additional props.
### How they work:
Take a component as an argument.
Return a new component that wraps the original component.
The new component can extend or modify the original component's behavior or props.
### Example Use Case:
A HOC can add a "loading" feature to a component, showing a loading message while data is fetched asynchronously. This way, the original component can focus on rendering the data while the HOC handles loading state management.





