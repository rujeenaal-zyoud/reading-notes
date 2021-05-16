# React and Forms
###### Some questions
1- **What is a ‘Controlled Component’?**
*controlled component is a react component that controls the values of input elements in a form using setState*

2 - **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them?**
*we should update the state with their responeses as soon as they enter them because the React take some time to update the state so if we did this after the submition maybe anonther compenent depends on these values will not work propely*

3- **How do we target what the user is entering if we have an event handler on an input field?**
*by using the (event.target.name)for that input filed.*
----------------------------------------------------------------------------------------
## Form
#### Controlled Components .
**In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().**

**We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.**
-----------------------------------------------------------------------
###### NOW LET'S GET SOME TAG THAT WE CAN USING IN HTML
#### The textarea Tag
**In HTML, a <textarea> element defines its text by its children:**

**In React, a <textarea> uses a value attribute instead. This way, a form using a <textarea> can be written very similarly to a form that uses a single-line input.**
----------------------------------------------------------------------
#### The select Tag
**In HTML, <select> creates a drop-down list. For example, this HTML creates a drop-down list of flavors**
EX:: 
![select](https://www.codegrepper.com/codeimages/react-select-tag.png)
------------------------------------------------------------------------

#### The file input Tag
**In HTML, an <input type="file"> lets the user choose one or more files from their device storage to be uploaded to a server or manipulated by JavaScript via the File API .**
------------------------------------------------------------------------
#### Handling Multiple Inputs
**When we need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of (event.target.name.)**
---------------------------------------------------------------------
#### The Conditional (Ternary) Operator
**Starting With the Basics — The if statement**
**Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.**
![ifconditional](https://scotch-res.cloudinary.com/image/upload/w_auto,q_auto:good,f_auto/v1562952581/jqctyinrganjts991d3w.jpg)
