[BACK](https://abdullahmou.github.io/reading-notes/)
## NumPy
![](https://miro.medium.com/max/765/1*cyXCE-JcBelTyrK-58w6_Q.png)
**NumPy**
* is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem,

### Lists Of Lists for CSV Data

* Import the csv library.
* Open the winequality-red.csv file.
  * With the file open, create a new csv.reader object.
    * Pass in the keyword argument delimiter=";" to make sure that the records are split up on the semicolon character instead of the default comma character.
  * Call the list type to get all the rows from the file.
  * Assign the result to wines.


### Numpy 2-Dimensional Arrays

is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.

### Using NumPy To Read In Files

It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function. We can use it to read in our initial data on red wines.

## Indexing NumPy Arrays

* We can use array indexing to select individual elements, groups of elements, or entire rows and columns.

* One important thing to keep in mind is that just like Python lists, NumPy is zero-indexed, meaning that the index of the first row is 0, and the index of the first column is 0.


## NumPy Array Operations

NumPy makes it simple to perform mathematical operations on arrays. This is one of the primary advantages of NumPy, and makes it quite easy to do computations.

**Single Array Math**

* If you do any of the basic mathematical operations (/, *, -, +, ^) with an array and a value, it will apply the operation to each of the elements in the array.

**Multiple Array Math**
* It’s also possible to do mathematical operations between arrays. This will apply the operation to pairs of elements.

**Broadcasting**
* Unless the arrays that you’re operating on are the exact same size, it’s not possible to do elementwise operations. In cases like this, NumPy performs broadcasting to try to match up elements. Essentially, broadcasting involves a few steps:

  * The last dimension of each array is compared.
      * If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
      * If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.
  * Continue checking dimensions until the shortest array is out of dimensions.


## NumPy Array Comparisons

NumPy makes it possible to test to see if rows match certain values using mathematical comparison operations like `<`, `>`, `>=`, `<=`, and `==`. 

## Reshaping NumPy Arrays

We can change the shape of arrays while still preserving all of their elements. This often can make it easier to access array elements.
some usuful function :

* numpy.transpose function:
* numpy.ravel function 
* numpy.reshape function
