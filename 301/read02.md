#  State and Props
 ##### The first thing we can convert a function component like Clock to a class in five steps:

-*Create an ES6 class, with the same name, that extends React.Component.*
*Add a single empty method to it called render().*
*Move the body of the function into the render() method.*
*Replace props with this.props in the render() body.*
*Delete the remaining empty function declaration.*

## Handling Events
![handling](https://static.javatpoint.com/tutorial/reactjs/images/react-events.png)
-----------------------------------------------------------------------------------------------------------
**Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:**

*React has its own event handling system which is very similar to handling events on DOM elements. The react event handling system is known as Synthetic Events. The synthetic event is a cross-browser wrapper of the browser's native event*
------------------------------------------------------------------------
**How handdle event in react?**
![how handle](https://vegibit.com/wp-content/uploads/2019/04/react-pass-event-arguments.png)
-----------------------------------------------------------------------
## Conditional Rendering
![Conditional](https://i.ytimg.com/vi/Xvc3MkkZnSQ/maxresdefault.jpg)
**The Conditional in React work as in JS also with render**
EX:
![EX](https://res.cloudinary.com/practicaldev/image/fetch/s--uFrIEIUm--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/08nsdwy9jrvu52e40g4p.PNG)
----------------------------------------------------------
### Inline If-Else with Conditional Operator
**Another method for conditionally rendering elements inline is to use the JavaScript conditional operator condition ? true : false.**
-------------------------------------------------
### Preventing Component from Rendering
**In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.**
-----------------------------------------------------------------------------
##### Element Variables
*We can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.*
 EX ::
 ![Element](https://res.cloudinary.com/practicaldev/image/fetch/s--EzLGRwgS--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/pd50euhxmawva1ns3y0a.png)
------------------------------------------------------------------
## Adding Lifecycle Methods to a Class
**In applications with many components, it’s very important to free up resources taken by the components when they are destroyed.**

**We can declare special methods on the component class to run some code when a component mounts and unmounts**




