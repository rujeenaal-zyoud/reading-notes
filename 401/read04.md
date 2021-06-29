# Express REST API

## Three real world use cases where you’d want to change the request with custom middleware
---------------------------------------------------------------------
1. Authenticate and authorization.
2. Error Handling.
3. Parameters validation.
-------------------------------------------------------
 #### The route handler is middleware?
 False
------------------------------------------------------------------

##### Route paths:
Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.

The characters ?, +, *, and () are subsets of their regular expression counterparts. The hyphen (-) and the dot (.) are interpreted literally by string-based paths.


#### Ways can a middleware function end the process and send data to the browser
 * response.send() .
 * response.render() .
 * response.json() .
 * response.redirect() .
 * res.download() .
 * res.end() .
 *  res.jsonp() .
 * res.sendFile() .
 * res.sendStatus() . 
 --------------------------------------------

 ### The point in the request lifecycle can you “inject” middleware
 *After client request and before response, in the middle of request and response cycle.*
 ------------------------------------------------------------

  #### What can cause express to error with “Request headers sent twice, cannot start a second response
  when we are already in the Body or Finished state, but some function tried to set a header or statusCode.

-----------------------------------------------------
#### We can do using express routing:

* Use express.Router() multiple times to define groups of routes.
* Apply the express.Router() to a section of our site using app.use().
* Use route middleware to process requests.
* Use route middleware to validate parameters using .param().
* Use app.route() as a shortcut to the Router to define multiple requests on a route.






