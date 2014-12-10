====================
Learn jQuery
====================

Chapter 1 About jQuery
====================

Chapter 2 JavaScript 101
====================

1. Getting Started
--------------------

2. Running Code
--------------------

  a. External
     
    <script src="/path/to/example.js"></script>
  
  b. Inline::
   
       <script>
       alert( "Hello World!" );
       </script> 

  c. Attributes

    This method is strongly discouraged::
      
      <!-- Inline code directly on HTML elements being clicked. -->
      <a href="javascript:alert( 'Hello World' );">Click Me!</a>
      <button onClick="alert( 'Good Bye World' );">Click Me Too!</button>

  d. Placement

    + If you are including JavaScript that doesn't access the elements on the page,
   
    you can safely place the script before the closing HTML <head> tag. 
    
    + However, if the code will interact with the elements on the page, you have to 
      
    make sure those elements exist at the time the script is executed

    + It is a common pattern to move scripts to the bottom of the page, prior to the
     
    closing HTML <body> tag

3. Syntax Basics
--------------------

4. Types
--------------------

5. Operators
--------------------

6. Conditional Code
--------------------

7. Loops
--------------------

8. Reserved Words
--------------------

9. Arrays
--------------------

10. Objects
--------------------

11. Functions
--------------------

12. Testing Type
--------------------

13. The "this" Keyword
--------------------

14. Scope
--------------------

15. Closures
--------------------

Chapter 2 Using jQuery Core
====================

Chapter 4 Events
====================

Chapter 5 Effects
====================

Chapter 6 Ajax 
====================

Chapter 7 Plugins 
====================

Chapter 8 Performance
====================

Chapter 9 Code Organization
====================

Chapter 10 jQuery UI
====================

Chapter 11 jQuery Mobile
====================
