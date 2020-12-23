
# Regular Expression

![](https://tutorial.eyehunts.com/wp-content/uploads/2018/09/Python-Regex-Regular-Expression-or-RE-Operations-Examples-.png)

* **regex** are a sequence of characters used to check whether a pattern exists in a given text (string) or not

## import

      import re

## Characters

* **.** 
  *  A period. Matches any single character except the newline character.

* **^** 
  *  A caret. Matches the start of the string.

* **$** 
  * - Matches the end of string.

* **[abc]** 
  * - Matches a or b or c.
* **[a-zA-Z0-9]** 
  * - Matches any letter from (a to z) or (A to Z) or (0 to 9).

* **\\** 
  * - Backslash. Perhaps, the most diverse metacharacter!!

* **\w** 
  * - Lowercase 'w'. Matches any single letter, digit, or underscore.
* **\W** 
  * - Uppercase 'W'. Matches any character not part of \w (lowercase w).

* **\s** 
  * - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.
* **\S** 
  * - Uppercase 'S'. Matches any character not part of \s (lowercase s). 

* **\d** 
  * - Lowercase d. Matches decimal digit 0-9.
* **\D** 
  * - Uppercase d. Matches any character that is not a decimal digit.

* **\t** 
  * - Lowercase t. Matches tab.
* **\n** 
  * - Lowercase n. Matches newline.
* **\r** 
  * - Lowercase r. Matches return.
* **\A** 
  * - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.
* **\Z** 
  * - Uppercase z. Matches only at the end of the string.

* **\b** 
  * - Lowercase b. Matches only the beginning or end of the word.

  ![](https://secureservercdn.net/160.153.137.210/ivc.7cc.myftpupload.com/wp-content/uploads/2019/12/BART457.png)
