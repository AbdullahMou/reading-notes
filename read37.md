# React

## React.js Fundamentals:

* Components are the building blocks of React. If you’re coming from an Angular background, components are very similar to Directives.
*  These components are defined either in pure JavaScript or they can be defined in what the React team calls “JSX”
* What makes React so convenient for building user interfaces is that data is either received from a component’s parent component, or it’s contained in the component itself. Before we jump into code, let’s make sure we have a high level understanding of components.

## Creating Component

## Adding State Component

* Each component has the ability to manage its own state and pass its state down to child components if needed.
* if you have a multi component hierarchy, a common parent component should manage the state and pass it down to its children components via props.

## Receiving State from Parent Component

* **props**  is the data which is passed to the child component from the parent component.
* This allows for our React architecture to stay pretty straight forward.
* Handle state in the highest most parent component which needs to use the specific data, and if you have a child component that also needs that data, pass that data down as props.
* the code that gets returned from our render method is a representation of what the real DOM should look like.
  * prop-types allow you to control the presence, or types of certain props passed to the child component. With propTypes you can specify that certain props are required or that certain props be a specific type.
  * defaultProps allow you to specify a default (or a backup) value for certain props just in case those props are never passed into the component.

## Component LifeCycle

* `componentDidMount` - Invoked once after the initial render. Because the component has already been invoked when this method is invoked, you have access to the virtual DOM if you need it. You do that by calling this.getDOMNode(). So this is the lifecycle event where you’ll be making your AJAX requests to fetch some data.*

* `componentWillUnmount` - This life cycle method is invoked immediately before a component is unmounted from the DOM. This is where you can do necessary clean up.

* `getDerivedStateFromProps` - Sometimes you’ll need to update the state of your component based on the props that are being passed in. This is the lifecycle method in which you’d do that. It’ll be passed the props and the state, and the object you return will be merged with the current state.
