lazy
====

A handy little javascript lazy loader. I wrote these helper functions because of the way that Rails concatenates assets in alphabetical order. It was becoming a nightmare to maintain the list of requires in the correct order. This solves that problem.

Usage
====

    lazydefine "Superclass", ->
      class Superclass
        ...
      
      Superclass
    
    lazydefine "MyClass", ["Superclass"], (Superclass) ->
      class MyClass extends Superclass
        ...
    
      MyClass
    
    lazyload "MyClass", (MyClass) ->
      ...
    
      

