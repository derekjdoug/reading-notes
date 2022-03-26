[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 13

## Local Storage

### The Past, Present, and Future of Local Storage for Web Applications

Native client applications have held advantages over web applications for storage for a long time.
Sure, web applications have cookies that are able to store small amounts of data, but there are several key disadvantages to relying on them too heavily.
They include.

1. Cookies are included with every HTTP request...even when not needed (this will slow down your web application needlessly)
2. Since they are included with every HTTP request, unencrypted data is being repeatedly transmitted, unless the entire app is served over SSL
3. Cookies are limited to 4 KB of data. Not enough to be overly useful or versatile, but enough to slow down your app

Instead, we want lots of storage space, on the client, that exists even after a page refresh, and that is also not transmitted to the server.

HTML5 is the key to making this happen.
*Before* HTML5, there were different solutions to increasing user storage on web applications, including: userData, dojox.storage, and Google Gears.
Unfortunately, these required the use of specific browsers or specific plugins to correctly function.

"HTML5 Storage" is known as **Web Storage**, **Local Storage**, or **DOM Storage** depending on the browser vendor.
This provides a way for web pages to store key/value pairs *locally*, without the need to transmit them to a remote web server, even if you navigate away from the page or close the browser and return to it later.
Crucially, it is implemented within web browsers natively, so there it is always available, even when third-party plugins would not be.

From JavaScript, you can detect whether or not the browser supports it with an example of the following code from [HTML5 Doctor](http://diveinto.html5doctor.com/storage.html):

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

```
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```

To use HTML5 Storage, you store and retrieve data based on a **named key**, which is a *string*.
The data can be of any type, however, it will be stored *as a string as well*, meaning you will need to use functions like `parseInt()` or `parseFloat()` to convert the data into the type you want.
You can also use event Listeners to programatically track when changes are made to the storage.

Examples and more can be found at: [HTML5 Doctor](http://diveinto.html5doctor.com/storage.html), where these notes were taken from.
