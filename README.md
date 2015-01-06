lazy
====

A handy little javascript lazy loader.

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
    
      

