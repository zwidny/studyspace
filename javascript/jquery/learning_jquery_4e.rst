====================
Learning jQuery Fourth Edition
====================


Chapter 1. Getting Started
====================

1. What jQuery does
--------------------

2. Why jQuery works well
--------------------

3. Making our first jQuery-powered web page
--------------------

4. Plain JavaScript versus jQuery
--------------------

5. Using development tools
--------------------

6. summary
--------------------

Chapter 2. Selecting Elements
====================

1. Understanding the DOM
--------------------

2. Using the $() function
--------------------
  
  In order to create a new jQuery object, we use the $() function

  The three primary building blocks of selectors are tag name, ID, and class

  +---------------+-------------+---------------+
  | Selector Type |  CSS        | jQuery |
  +---------------+-------------+---------------+
  | Tag name      |  p{}        | $('p') |
  +---------------+-------------+---------------+
  | ID            | #a-id {}    | $('#a-id') |
  +---------------+-------------+---------------+
  | Class         | .a-class {} | $('.a-class') |
  +---------------+-------------+---------------+

3. CSS selectors
--------------------

4. Attribute selectors
--------------------

  e.g.: $('img[alt]')

  a. Styling links

    Attribute selectors accept a wildcard syntax inspired by regular 
    
    expressions for identifying the value at the beginning ( ^ ) or 
    
    end ( $ ) of a string

    e.g.::
        $(document).ready(function() {
            $('a[href^="mailto:"]').addClass('mailto');
         });

5. Custom selectors
--------------------

6. DOM traversal methods
--------------------

7. Accessing DOM elements
--------------------

8. Summary
--------------------

9. What I need improve
--------------------

  a. CSS Selector

  b. jQuery DOM traversal methods

 
Chapter 3. Handling Events
====================


