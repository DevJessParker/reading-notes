# State and Props

## Key Terms and Concepts

Term | Definition
----- | -----
lifecycle events | methods that can be called on a React component to update the application state



- Lifecycle phases:
  - Mounting, Updating, Unmounting
  - Pre-Commit stage allows access to read the DOM
  -Unmounting removes from DOM

-Constructor:
  -Called before the Mounting phase.
  -Props will be undefined if super(props) is not called.
  -this.state used to assign state

-Render: 
  -Required method for class component.
