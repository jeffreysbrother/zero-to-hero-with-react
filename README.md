> To begin, run `npm install` to install dependencies ... and `npm run start-webpack-server` to start the server.

React is a JavaScript library that helps you build user interfaces. It is so popular because it presents a new paradigm for doing this.

A component, generally speaking, is an independent piece of the application. One advantage of thinking in terms of components is reusability. Components can also be shared. Many component libraries already exist.

React is the "V" in MVC. It can be connected with a state management library such as Redux.

Benefits of using React (taken from multiple sources):

* updating the React Virtual DOM is a more efficient way of making changes to the view of a web application.
* unidirectional data binding
* the use of components

A React component:

* a render function (the only function that is required in a React component)
* within the render function, optional JSX (which is compiled by Babel into JS functions, and which must have only one parent element)
* has state

In this tutorial, which may or may not be out of date, it looks like they're creating components like this:

```js
var App = React.createClass({
  render : function() {
    return (
      // start JSX
      <div>
        <div id="header"></div>
        <div className="container">
          <div className="column">
            // and this appears to be another component
            <InboxPane />
          </div>
          <div className="column"></div>
          <div className="column"></div>
        </div>
      </div>
      // end JSX
    )
  }
});
```
###CSS Scoping

Nothing horribly interesting here. Apparently it is common to wrap the JSX in a containing div and to simply use child/descendent selectors in CSS to target ONLY the contents of that component. If I'm not mistaken, Angular has a more interesting way of accomplishing this.

###Component Lifecycle

Every component has a lifecycle. 
