[BACK](https://abdullahmou.github.io/reading-notes/)
# List Comprehensions

![Comprehensions](https://files.realpython.com/media/List-Comprehensions-in-Python_Watermarked.39cf85bdd5d0.jpg)

* It consists of brackets containing an expression followed by a for clause,
* then zero or more for or if clauses.
* The expressions can be anything, meaning you can put in all kinds of objects in lists.
* The result will be a new list resulting from evaluating the expression in the
context of the for and if clauses which follow it.

* The list comprehension always returns a result list.

                new_list = []
                for i in old_list:
                    if filter(i):
                        new_list.append(expressions(i))

## Syntax

         new_list = [expression(i) for i in old_list if filter(i)]

**new_list**

* The new list (result).

**expression(i)**

* Expression is based on the variable used for each element in the old list.

**for i in old_list**

* The word for followed by the variable name to use, followed by the word in the old list.

**if filter(i)**

* Apply a filter with an If-statement.
