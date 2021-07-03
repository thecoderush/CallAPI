# All possible ways of making an API call in JavaScript.
https://levelup.gitconnected.com/all-possible-ways-of-making-an-api-call-in-plain-javascript-c0dee3c11b8b

In JavaScript, it was really important to know how to make HTTP requests and retrieve the dynamic data from the server/database.

JavaScript provides some built-in browser objects and some external open  source libraries to interact with the APIs.

Here are the possible ways to make an API call:

    1. XMLHttpRequest
    2. fetch
    3. Axios
    4. jQuery

## XMLHttpRequest

Before ES6 comes out, the only way to make an HTTP request in JS was XMLHttpRequest. It is a built-in browser object that allows us to make HTTP requests in JS from the browser.

    to check to browser built-in object : 

    console.log(window)

    you can see the global properties XMLHttpRequest that can be used directly

So how can we make the request ?

JSONPlaceholder https://jsonplaceholder.typicode.com/ is a free online REST API that you can use whenever you need some fake data.

    ...

By default we receive the response in the string format, we need to parse into JSON. 

XMLHttpRequest was deprecated in ES6 by the introduction of fetch. But still, we are using XMLHttpRequest when we need to work with old browsers and don't want polyfills.

## Fetch

Fetch allows you to make an HTTP request in a similar manner as XMLHttpRequest but with a straightforward interface by using promises.

It's not supported by older browsers (can be polyfilled), but very well supported amoung the modern ones. We can make an API call by using fetch in two ways.

    * Method 1
    * By using Async and Await

    ...

The fetch API is very powerful. We can easily send AJAX requests using the browser fetch API. The major disadvantage of fetch API is error handling.

## Axios

Axios is an open-source library for making HTTP requests and provides many great features, and it works both in browsers and Node.js. 

It is a promise-based HTTP client that can be used in plain JS and advanced frameworks like React, VueJS and Angular.

It support all modern browsers, includes support for IE8 and higher.

Installation:
    
If you are using any one of the package managers like npm or yarn.
    
    $ npm install axios 
    or
    $ yarn add axios

And include it in HTML file like this 

    <script src="./node_modules/axios/dist/axios.min.js"></script>

The easiest way to include Axios is by using external CDN:

    <script src="https://unpkg.com/axios/dist/axios.min.js"></script>

Now you can start sending HTTP request by including the following script in your HTML file.

    ...

The following are the advantages of Axios 

    1. Axios performs automatic transformations and returns the data in JSON format.
    
    2. Better error handling
    
    3. Axios has a wide range of supported browsers.

## jQuery

The $.ajax method takes many parameters, some of which are required and others optional. It contains two callback functions success and error to handle the response received.  

    ...

### Conclusion

Most of the real-time applications are using Axios to make HTTP requests.

Axios is very easy and open-source library for making HTTP requests.

I have covered the most popular ways to make HTTP requests in JS.

For your convenience, I am adding source code here https://github.com/jayanthbabu123/all-possible-ways-making-api-call-javascript .

No one's perfect. Please comment on any suggestions and enhancements.

Thanks for your time.