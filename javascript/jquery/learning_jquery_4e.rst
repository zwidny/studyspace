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
  | Selector Type |  CSS        | jQuery        |
  +===============+=============+===============+
  | Tag name      |  p{}        | $('p')        |
  +---------------+-------------+---------------+
  | ID            | #a-id {}    | $('#a-id')    |
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

1. Performing tasks on page load
--------------------

  a. Timing of code execution
    
    The **window.onload** event fires when a document is completely downloaded 
    to
   
    the browser.


    The **$(document).ready()** is invoked when the DOM is completely ready for
   
    use

  b. Handling multiple scripts on one page

  c. Alternate syntax for .ready()

    When we pass in a function as the argument to $() , jQuery performs an
   
    implicit call to .ready(d. Passing an argument to the .ready() callback

    e.g.::
      $(document).ready(function() {
      // Our code here...
      });

      <=>

      $(function() {
      // Our code here...
      });


  d. Passing an argument to the .ready() callback

    we need a way to prevent collisions between diff jquery library uses.

2. Handling simple events
--------------------

  a. A simple style switcher

    we'll introduce the **.on()** method. This method allows us to specify
   
    any DOM event and to attach a behavior to it.

  b. Enabling the other buttons

  c. Making use of the event handler context

  d. Consolidating code using the event context

  e. Shorthand events

  f. Showing and hiding advanced features

    JQuery provides an easy way for us to add or remove a class depending on
   
    whether that class is already present—the **.toggleClass()** method

3. Event propagation
--------------------

  .hover()

4. Altering the journey – the event object
--------------------

  a. Event targets

  b. Stopping event propagation

    event.stopPropagation();

  c. Preventing default actions

    event.preventDefault()

  d. Delegating events

  f. Using built-in event-delegation capabilities

5. Removing an event handler
--------------------

  a. Giving namespaces to event handlers

  b. Rebinding events

6. Simulating user interaction
--------------------

7. Summary
--------------------

Chapter 4. Styling and Animating
====================

1. Modifying CSS with inline properties
--------------------

2. Hiding and showing elements
--------------------

3. Effects and duration
--------------------

  a. Speeding in

  b. Fading in and fading out

  c. Sliding up and sliding down

  d. Toggling visibility

4. Creating custom animations
--------------------

5. Simultaneous versus queued effects
--------------------
