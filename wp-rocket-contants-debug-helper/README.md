# WP Rocket | Constants Debug Helper

Checks for defined constants (`WP_CACHE`, `DONOTCACHEPAGE`, `DONOTMINIFY`, `DONOTMINIFYCSS`, `DONOTMINIFYJS`) and prints their values as an HTML comment in the footer of the HTML source code.

## How to use
- Once you have installed and activated the plugin, clear the cache.
- Open any page of your website in an anonymous browser window (where you are not a logged-in WordPress user).
- Switch to source view in your browser.
- Look for an HTML comment starting with `WP ROCKET DEBUG` towards the bottom of the source code view.
- Each of the above constants gets listed in the comment.

## Sample output in HTML source view

```
<!--
####################################################

## WP ROCKET DEBUG ##
(HTML minification disabled "on the fly" by this helper plugin.)

- constant WP_CACHE is true

- constant DONOTCACHEPAGE is true

- constant DONOTMINIFY is true

- constant DONOTMINIFYCSS is not defined

- constant DONOTMINIFYJS is not defined

####################################################
-->
```

To be used with:
* any setup

Last tested with:
* WP Rocket 2.9.x
* WordPress 4.7.x
