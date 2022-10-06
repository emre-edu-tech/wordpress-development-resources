# General Object Oriented Concepts
## Namespace
- This is a way of grouping classes in object oriented programming.
- Behaves like a virtual directory that holds the related classes.
- Allows you to have two or more classes with the same name in different namespaced directories.
- While instantiating or using the classes, "namespace" or "use" keywords can be used.

## Autoloader
- Loading the classes or interfaces automatically. include_once or required_once functions become unnecessary.
- spl_autoload_register()
    - Registers any number of autoloaders
    - Loads the classes in a given folder without declaring class names one by one.

## Trait
- Normally only properties and methods can be inherited from parent class to child by extending the parent.
- If the child class should also be inherited by one another class then chain of inheritance will be occured.
- To avoid from the chain of inheritance and use the methods and properties of different/independent classes, traits will be the answer in PHP.
- A trait is similar to a class, but only intended to group functionality in a consistent way. (Like putting all the string related methods into String Helper trait)
- It is not possible to instantiate a trait. It can only be used by using "use" keyword inside a traditional class.
- After adding the trait in a traditional class, then this class can access the methods and properties of that trait.
- Traits can be added both inside and outside of class block using the "use" keyword.