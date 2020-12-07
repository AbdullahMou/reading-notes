[BACK](https://abdullahmou.github.io/reading-notes/)

# Scoping

* Global scope:
  * The names that you define in this scope are available to all your code.

* Local scope:
  *  The names that you define in this scope are only available or visible to the code within the scope.

## Names and Scopes in Python


|Operation	|Statement|
|---------------|-----------------|
|Assignments|	x = value|
|Import operations	|import module or from module import name|
|Function definitions|	def my_func(): ...|
|Argument definitions in the context of functions|	def my_func(arg1, arg2,... argN): ...
|Class definitions|	class MyClass:|

## Python Scope vs Namespace

*  the concept of scope is closely related to the concept of the namespace.

# Using the LEGB Rule for Python Scope

* Python resolves names using the so-called LEGB rule
  * Local (or function) scope
  * Enclosing (or nonlocal) scope
  * Global (or module) scope
  * Built-in scope

### Functions: The Local Scope
  
* The local scope or function scope is a Python scope created at function calls.  

### Nested Functions: The Enclosing Scope

*  nonlocal scope is observed when you nest functions inside other functions.
*  It takes the form of the local scope of any enclosing function’s local scopes

### Modules: The Global Scope

* From the moment you start a Python program, you’re in the global Python scope.

