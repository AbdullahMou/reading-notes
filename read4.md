# Classes and Objects
![](https://www.gangboard.com/wp-content/uploads/2019/05/python-class-and-object.jpg)

![](https://i.ytimg.com/vi/4dqlSk_RPmI/maxresdefault.jpg)

* Objects are an encapsulation of variables and functions into a single entity.
* Objects get their variables and functions from classes.
* Classes are essentially a template to create your objects.

## Accessing Object Variables

![](https://files.realpython.com/media/Pointers-in-Python_Watermarked.d8551f0cd1d2.jpg)

* To access the variable inside of the created object
  * `class MyClass:`
`    variable = "blah"`
 `   def function(self):`
  `      print("This is a message inside the class ")`
`myobjectx = MyClass()`
`myobjectx.variable`

* So for instance the below would output the string "blah":
  * `print(myobjectx.variable)`

* To access a function inside of an object 
  * `myobjectx.function()`

# Thinking Recursively

![](https://miro.medium.com/max/12000/0*uJOJz1qoOx7drig4)

## Recursive Functions in Python

![](https://www.bogotobogo.com/cplusplus/images/quiz/recursion_factorial.png)

* A recursive function is a function defined in terms of itself via self-referential expressions.
* This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result.
* All recursive functions share a common structure made up of two parts: base case and recursive case.
  * Decompose the original problem into simpler instances of the same problem. This is the recursive case:
    * `n! = n x (n−1) x (n−2) x (n−3) ⋅⋅⋅⋅ x 3 x 2 x 1`
  * those subproblems must eventually become so simple that they can be solved without further subdivision
    * `  n! = n x (n−1) x (n−2) x (n−3)!`


## Maintaining State

* When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:
  * Thread the state through each recursive call so that the current state is part of the current call’s execution context
  * Keep the state in global scope
  * A demonstration should make things clearer. 

## Recursive Data Structures in Python


