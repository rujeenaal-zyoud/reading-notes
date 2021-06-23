# Node Ecosystem, TDD, CI/CD
---------------------------------------------------------------

### TDD (Test-driven development)

refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).


**It can be succinctly described by the following set of rules:**

* write a “single” unit test describing an aspect of the program
* run the test, which should fail because the program lacks that feature
* write “just enough” code, the simplest possible, to make the test pass
* “refactor” the code until it conforms to the simplicity criteria
*  repeat, “accumulating” unit tests over time

-----------------------------------------------------------------------------

 #### CI/CD (continuous integration/contiuous delivery)**

*CI/CD is a method to frequently deliver apps to customers by introducing automation into the stages of app development. The main concepts attributed to CI/CD are continuous integration, continuous delivery, and continuous deployment. CI/CD is a solution to the problems integrating new code can cause for development and operations teams (AKA "integration hell")*

-----------------------------------------------------------------------
 #### Review, Research, and Discussion**

 
1. ###### what Array.map() does? 
allows you to iterate over an array and modify its elements using a callback function. The callback function will then be executed on each of the array's elements.

2. ###### what Array.reduce() does?
 used to reduce the array to a single value and executes a provided function for each value of the array (from left-to-right) and the return value of the function is stored in an accumulator.

3. code snippets showing how to use superagent to fetch data from URL and log the results.

##### promises
 **let say that we havea code that take some time and another one that depends on the result from the first , here promis is the javascript object that links between the previous codes to work properly.**

#### Are all callback functions considered to be Asynchronous?
 *callbacks don't have anything to do with the async concept at all. They're just regular functions, and they don't know or care whether they're going to be called asynchronously or not. so a callback can be used synchronously or asynchronously.*

 





