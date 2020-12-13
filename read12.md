[BACK](https://abdullahmou.github.io/reading-notes/)
# pandas

## Object creation

* Creating a Series by passing a list of values, letting pandas create a default integer index
  * `s = pd.Series([1, 3, 5, np.nan, 6, 8])`

## Viewing data

* Here is how to view the top and bottom rows of the frame:
  * ` df.head()`</br>
  * `df.tail(3)`

## Selection

**Getting**

* Selecting a single column, which yields a Series, equivalent to `df.A`:
  * ` df['A']`

* Selecting via [], which slices the rows.

  * ` df[0:3]`  

**Selection by label**

* For getting a cross section using a label:
  * `df.loc[dates[0]]`
  * ` df.loc[:, ['A', 'B']]`

**Selection by position**

* Select via the position of the passed integers:

  * ` df.iloc[3]`
  * `df.iloc[3:5, 0:2]`
  * `df.iloc[[1, 2, 4], [0, 2]]`

## Merge 

**Concat**

* Concatenating pandas objects together with concat():
  * `df = pd.DataFrame(np.random.randn(10, 4))`
  ` pieces = [df[:3], df[3:7], df[7:]]`
  `pd.concat(pieces)`

**Join**

* SQL style merges. See the Database style joining section.
    * ` left = pd.DataFrame({'key': ['foo', 'foo'], 'lval': [1, 2]})`
    ` right = pd.DataFrame({'key': ['foo', 'foo'], 'rval': [4, 5]})`
    `pd.merge(left, right, on='key')`

## Grouping

* By “group by” we are referring to a process involving one or more of the following steps:

  * **Splitting** the data into groups based on some criteria

  * **Applying** a function to each group independently

  * **Combining** the results into a data structure
