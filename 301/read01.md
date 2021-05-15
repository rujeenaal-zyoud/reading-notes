
# Introduction to React and Components
#### What Is React?
**React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”**
**Notes**

*Also we have two of react component 1 class  2 type   each compnent take a parameters*

*The React Devtools extension for Chrome and Firefox lets you inspect a React component tree with your browser’s developer tools.*
------------------------------------------------------------------
#### Introducing JSX

**JSX comes with the full power of JavaScript. You can put any JavaScript expressions within braces inside JSX. Each React element is a JavaScript object that you can store in a variable or pass around in your program.**
###### Why using JSX
**React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.**
-----------------------------------------------------------------------------
#### Rendering Elements
- **The first of all meaning render it's show the element in our page by using  DOM JS**
-**Elements are the smallest block of react app**
-**There is deferent between DOM elements and React elements because react element is a plain of object**
 EX::
 ![image](https://miro.medium.com/max/2680/1*mXjNHOx9bbQ5D4sSUAX2Lg.png)
--------------------------------------------------------------------------------------------
###### NOTES
*React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.*
*React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.*
