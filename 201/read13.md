# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS
 **Web Storage is used for storing data on the client-side. So the data will be available even when the page is  refreshed.**
-----------------------------------------------------------------------------------------------
 *We have 2 type of storge*::
## Local storage
**Web storage objects localStorage and sessionStorage allow to save key/value pairs in the browser.**
**Every browesr have a cookie**
**Previously before Web Storage came into play, the only way of storing the data on the client-side was using cookies, but the cookies are some disadvantages of using like storge limit**
## Session Storage :
**Session Storage is for per browser tab. So data stored in one browser tab will not be accessible in another tab**
------------------------------------------------------------------------------
##### Web Storage interfaces
* Storage :
Allows you to set, retrieve and remove data for a specific domain and storage type (session or local.)
The Web Storage API extends the Window object with two new properties 

* Window:The Web Storage API extends the Window object with two new properties — Window.sessionStorage and Window.localStorage — which provide access to the current domain's session and local Storage objects respectively, and a Window.onstorage event handler that fires when a storage area changes (e.g. a new item is stored.)


 * StorageEvent
The storage event is fired on a document's Window object when a storage area changes by using JS.

 *A different Storage object is used for the sessionStorage and localStorage for each origin — they function and are controlled separately.*


 ###### notes
  * Both Local and Session Storage have a storage limit of 5MB each.
  * we can also clear the local storage data programmatically
  *  we can add event is fired on the window object whenever setItem(), removeItem(), or clear()


  
  ![img](https://lh3.googleusercontent.com/proxy/misjTAnaINkdS1mbhslObTAF8dQ48-Y1NmwWKpeUUw-QgR2ZiltZNkKJmJrA8tU8xJ7W-u6z_Q8_EOQbpyff1Bv_5OdvznX_g4i8z8F9jltcqoFB)