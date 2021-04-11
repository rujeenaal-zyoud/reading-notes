# Error Handling & Debugging
**first of all what error mean?**
**error mean something wrong in our code may of mistake from Lack of attention or logical error by missing point in project code**

--------------------------------------------------------------------------
#### There are two types of JavaScript error:

-Syntax Error: Occurs when there is a mistake in the way the code is written; for example, a typo or missing character.
-Runtime error: Occurs when the script is unable to complete its instructions; for example, if a specified object cannot be found.
**avaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error**

1-ORDER OF EXECUTION :*this mean order of statement it mean some methode depend in another varible or methode so the order is important to solve it the JS have EXECUT.ION CONTEXTS it message show by interputer the code in js*
2-XECUTION CONTEXT & HOISTING:*by having two PREPARE and EXECUTE this mean the varible in scope of code the interpreter in JS , each execution context has its own variables object.  Each execution context can also access its parent's v a ri ables object*

---------------------------------------------------------------------------
**So we need to understand the error to solve it  when error hapend the js  generate exception. At that point error by using**
- *consol log in browser*
-*error objects can help you find where your mistakes are and browsers have tools to help you read them.*
-*exception message*
-*Object error*: this have alot of type such as 
1-Syntax Error 
2-Ref erenceError 
3-Ev alError 
4-NaN
5- error
-------------------------------------------------------------------------------------
**We can solve the error in the code from browser or by using TRY, CATCH, FINALLY and the main processing for solve the error by depugging**
-----------------------------------------------------------------------------------------------
#### Note for me 
 I have learned in Tuesday the ERRORS in JS what the type of error and what the message that appeared when the error happen also how i can solve that error ever it logically error or by syntax error.

Type of error
1-first of all the undefined error it mean the JS do housing the declaration for variable that start with var name ="ruj" when consol.log this before declaration it will be undefined
but if we declaration with let name="ruj" here it will also be undefended but without housing the deceleration.

2- when change data that declaration as const like const name="ruje"; name ="fg" it will show Uncaught Type error because we change in constant var

3- reference error  like declare var but without assign any data to it so it will nt show a error it undefined


4- range error  like :   let arr=[1,2,3,4,5]; arr.length=90**99;    it mean trying to do something outside of range  like number out of values


5- Syntax Error  like let car fg ="bmw" then we will see a syntax error by forget put () /; or put space in declaration 

6- Scopes  it mean when declaration something in it then used the var out of that scope it will be in NAN error like function or for or object 