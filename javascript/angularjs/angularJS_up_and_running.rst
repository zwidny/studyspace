====================
AngularJS Up and Running
====================


Introduction
====================

Online Resources
--------------------

+ The Official AngularJS API Documentation

+ The Official AngularJS Developer Guide

+ The AngularJS PhoneCat Tutorial App

+ ngModules: A list of all known open source AngularJS modules

+ Egghead.io: Great AngularJS video tutorials


Chapter 1. Introducing AngularJS
====================

Introducing AngularJS
--------------------

What Is MVC (Model-View-Controller)?
~~~~~~~~~~~~~~~~~~~~

AngularJS Benefits
~~~~~~~~~~~~~~~~~~~~

The AngularJS Philosophy
~~~~~~~~~~~~~~~~~~~~

+ Data-driven(via data-binding)

+ Declarative

+ Separate your concerns

+ Dependency Injection

+ Extensible

+ Test first, test again, keep testing
  Karma, Protractor


Starting Out with AngularJS
--------------------

Conclusion
--------------------


Chapter 2. Basic AngularJS Directives and Controllers 
====================

AngularJS Modules
--------------------

Define a module
~~~~~~~~~~~~~~~~~~~~

+ angular.module('moduleName', []);

  The first argument to the module function in AngularJS is the name of the module

  The second argument is an array of module names that this module depends on

  e.g.::
    angular.module('noteApp', ['modules1', 'module2']);

+ a complete example to make sense of this::
    <html ng-app="noteApp">
    <head>
      <title>Hello AngularJS Modules</title>
    </head>
    <body>
      Hello {{1 + 1}nd time AngularJS
      <script src=""></script>
      <script type="text/javascript">
        angular.module();
      </script>
    </body>
    </html>


Creating Our First Controller
--------------------

Working with and Displaying Arrays
--------------------

More Directives
--------------------

Working with ng-repeat
--------------------

Conclusion
--------------------



