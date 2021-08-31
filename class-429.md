Django Best Practices: Custom User Model
By Will Vincent  Dec 7, 2020 8 Comments
Django ships with a built-in User model for authentication and if you'd like a basic tutorial on how to implement log in, log out, sign up and so on see the Django Login and Logout tutorial for more.

However, for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

But how to implement one? The official documentation example is not actually what many Django experts recommend using. There is a far easier yet still powerful approach to starting off new Django projects with a custom user model which I'll demonstrate here.


djangox 
djangox is a template with these features:
rocket Features
Django 3.1 & Python 3.8
Install via Pip, Pipenv, or Docker
User log in/out, sign up, password reset via django-allauth
Static files configured with Whitenoise
Styling with Bootstrap v4
Debugging with django-debug-toolbar
DRY forms with django-crispy-forms