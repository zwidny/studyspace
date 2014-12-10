====================
Learning jQuery, 4e
====================


Chapter 1. Getting Started
====================

1. What jQuery does
--------------------

  + Access elements in a document

  + Modify the appearance of a web page

  + Alter the content of a document

  + Respond to a user's interaction

  + Animate changes being made to a document

  + Retrieve information from a server without refreshing a page

  + Simplify common JavaScript tasks

2. Why jQuery works well
--------------------

  + Leverage knowledge of CSS

  + Support extensions

  + Abstract away browser quirks

  + Always work with sets

  + Allow multiple actions in one line

3. Making our first jQuery-powered web page
--------------------

  a. Downloading jQuery

  b. Deciding on the version of jQuery to use

  c. Setting up jQuery in an HTML document

  d. Adding our jQuery code

  e. Finding the poem text

  f. Injecting the new class

  g. Executing the code

  h. The finished product

4. Plain JavaScript versus jQuery
--------------------

5.Using development tools
--------------------

  a. Chrome Developer Tools

Chapter 2. Selecting Elements
====================

1. Understanding the DOM
--------------------

  The DOM serves as the interface between JavaScript and a web
  page;
 
  it provides a representation of the source HTML as a network
  of 
  
  objects rather  than as plain text.

2. Using the $() function
--------------------

  In order to create a new jQuery object, we use the $() function

3. CSS selectors
--------------------

4. Attribute selectors
--------------------

5. Custom selectors
--------------------

  a. Styling alternate rows 

    Well, just as with the :eq() selector, the **:even** and **:odd** selectors
   
    use JavaScript's native zero-based numbering

  b. Finding elements based on textual content

    All we have to do is add a line to our jQuery code using the :contains() 
    
    selector

  c. Form selectors::
    
    :input      Input, text area, select, and button elements
    :button     Button elements and input elements with a type
                attribute equal to button
    :enabled    Form elements that are enabled
    :disabled   Form elements that are disabled
    :checked    Radio buttons or checkboxes that are checked
    :selected   Option elements that are selected

6. DOM traversal methods
--------------------

  + .filter() --> $('tr').filter(':even').addClass('alt');

  a. Styling specific cells

      + .next() --> $('td:contains(Henry)').next().addClass('highlight');
        
      + .nextAll()

      + .prev()

      + .prevAll()

      + .siblings()

      + .addBack()

      + .parent()

      + .children()

  b. Chaining

7. Accessing DOM elements
--------------------

  var myTag = $('#my-element').get(0).tagName;

  var myTag = $('#my-element')[0].tagName;

Chapter 3. Handling Events
====================

1. Performing tasks on page load
--------------------

  a. Timing of code execution

    + $(document).ready()

    + window.onload

  b. Handling multiple scripts on one page

  c. Alternate syntax for .ready()
    
    $(document).ready() <==> $()

  d. Passing an argument to the .ready() callback

2. Handling simple events
--------------------

  a. A simple style switcher

  b. Consolidating code using the event context

  c. Shorthand events

  d. Showing and hiding advanced features

3. Event propagation
--------------------

  

4. Altering the journey – the event object
--------------------

5. Removing an event handler
--------------------

6. Simulating user interaction
--------------------

Chapter 4. Styling and Animating
====================

Chapter 5. Manipulating the DOM
====================

Chapter 6. Sending Data with Ajax
====================

Chapter 7. Using Plugins
====================

Chapter 8. Developing Plugins
====================

Chapter 9. Advanced Selectors and Traversing
====================

Chapter 10. Advanced Events
====================

Chapter 11. Advanced Effects
====================

Chapter 12. Advanced DOM Manipulation
====================

Chapter 13. Advanced Ajax
====================
