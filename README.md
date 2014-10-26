freedomjs-social-publiclog
==========================

A freedom.js social provider backed by a public writable log

The log used is passed in to the login function.
An example of a valid implementation of a public log implementing the expected get and append
interface is at

https://script.google.com/d/1RHD35GMcgVlzd3vw4rlb0Sgfegmw9ksKoUriL8V72eo3Uh1vuDe4wV50/edit?usp=sharing

The features expected of the final published url are:
* A get request, (optionally specifying a 'dest' query filter) returns recently appended objects.
* A post request, specifying src, dest, and msg query parameters will append a row.

In addition, the interface expects a JSONP based callback structure, which can be set in a
callback parameter.
