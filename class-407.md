# Python Scope & the LEGB Rule:
The concept of scope rules how variables and names are looked up in your code. 


The letters in the acronym LEGB stand for Local, Enclosing, Global, and Built-in scopes. 


    What scopes are and how they work in Python
    Why it’s important to know about Python scope
    What the LEGB rule is and how Python uses it to resolve names
    How to modify the standard behavior of Python scope using global and nonlocal
    What scope-related tools Python offers and how you can use them



In programming, the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on. A name will only be visible to and accessible by the code in its scope. Several programming languages take advantage of scope for avoiding name collisions and unpredictable behaviors. Most commonly, you’ll distinguish two general scopes:

    Global scope: The names that you define in this scope are available to all your code.

    Local scope: The names that you define in this scope are only available or visible to the code within the scope.

Scope came about because early programming languages (like BASIC) only had global names. With this kind of name, any part of the program could modify any variable at any time, so maintaining and debugging large programs could become a real nightmare. To work with global names, you’d need to keep all the code in mind at the same time to know what the value of a given name is at any time. This was an important side-effect of not having scopes.

Some languages like Python use scope to avoid this kind of problem. When you use a language that implements scope, there’s no way for you to access all the variables in a program at all locations in that program. In this case, your ability to access a given name will depend on where you’ve defined that name.


