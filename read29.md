# Django Best Practices
## Setup
* To start, create a new Django project from the command line. We need to do several things:

  * create and navigate into a dedicated directory called accounts for our code
  * install Django
  * make a new Django project called config
  * make a new app accounts
  * start the local web server
  
  ## Custom User Model
* Creating our initial custom user model requires four steps:

  * update config/settings.py
  * create a new CustomUser model 
  * create new UserCreation and UserChangeForm
  * update the admin

## Templates/Views/URLs
* **Our goal** 
  * is a homepage with links to log in, log out, and sign up. Start by updating settings.py to use a project-level templates directory. 
* **Then**
  * set the redirect links for log in and log out, which will both go to our home template. Add these two lines at the bottom of the file.
* **Then create templates**

## Conclusion
* Now that our custom user model is configured you can easily and at any time add additional fields to it. See the Django docs for further instructions.

* You can also check out DjangoX, which is an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.

