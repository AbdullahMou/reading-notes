# Django Forms

## Overview:

* An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server.
* Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on.
* Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

## HTML Forms

* action: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL.
* method: The HTTP method used to send the data: post or get.
  * The POST method should always be used if the data is going to result in a change to the server's database because this can be made more resistant to cross-site forgery request attacks.
  * The GET method should only be used for forms that don't change user data (e.g. a search form). It is recommended for when you want to be able to bookmark or share the URL.

## Django form handling process

* Display the default form the first time it is requested by the user.
* Receive data from a submit request and bind it to the form.
* Clean and validate the data.
* If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.
* If all data is valid, perform required actions (e.g. save the data, send an email, return the result of a search, upload a file, etc.)
* Once all actions are complete, redirect the user to another page.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/05/Django-forms.jpg)
