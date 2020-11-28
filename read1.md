[BACK](https://abdullahmou.github.io/reading-notes/)

## Pain and Suffering

* The pain is the price
* Suffering is pain without purpose
* Find the common thread that makes the pain worthwhile

## Big O notation
![](https://miro.medium.com/max/1200/1*s_NeM4zktzrHNBY45VLs-A.png)
* the grounding in Mathematics are important for Computer Science

* O(1) describes an algorithm that will always execute
  * `bool IsFirstElementNull(IList<string> elements)`</br>
    `{ return elements[0] == null;}`

* O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.
![](https://miro.medium.com/max/1097/1*ArzWC4bV3d6bDIFbZOSGkw.png)
  * `bool ContainsValue(IList<string> elements, string value)`</br>
`{  foreach (var element in elements)`</br>
 `   {`</br>
 `  if (element == value) return true;}`</br>
  `  return false;`</br>
  `}`

* O(N2) represents an algorithm whose performance is directly proportional to the square of the size of the input data set.
* This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N3), O(N4)
![](https://www.101computing.net/wp/wp-content/uploads/Big-O-Notation-Polynomial-Algorithm.png)</br>
  * ` bool ContainsDuplicates(IList<string> elements)`
`{`</br>
`    for (var outer = 0; outer < elements.Count; outer++)`</br>
 `   {`</br>
  `      for (var inner = 0; inner < elements.Count; inner++)`</br>
   `     {`</br>
    `        // Don't compare with self`</br>
     `       if (outer == inner) continue;`</br>

 `           if (elements[outer] == elements[inner]) return true;`</br>
  `      }`</br>
   ` }`</br>

`return false;`</br>
`}`

* O(2N) denotes an algorithm whose growth doubles with each additon to the input data set. The growth curve of an O(2N) function is exponential - starting off very shallow, then rising meteorically
![](https://www.101computing.net/wp/wp-content/uploads/Big-O-Notation-Exponential-Algorithm.png)
  * `int Fibonacci(int number)`</br>
`{`</br>
 `   if (number <= 1) return number;`</br>

  `  return Fibonacci(number - 2) + Fibonacci(number - 1);`</br>
`}`

### The iterative halving

* Binary search is a technique used to search sorted data sets
* It works by selecting the middle element of the data set, essentially the median, and compares it against a target value
* If the values match it will return success. If the target value is higher than the value of the probe element it will take the upper half of the data set and perform the same operation against it
* Likewise, if the target value is lower than the value of the probe element it will perform the operation against the lower half
* It will continue to halve the data set with each iteration until the value has been found or until it can no longer split the data set
![](https://www.topcoder.com/wp-content/uploads/2017/07/binary-search.png)
