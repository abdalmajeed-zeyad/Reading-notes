Enriching Your Python Classes With Dunder (Magic, Special) Methods




Object Initialization: __init__

Right upon starting my class I already need a special method. To construct account objects from the Account class I need a constructor which in Python is the __init__ dunder:



Object Representation: __str__, __repr__

It’s common practice in Python to provide a string representation of your object for the consumer of your class (a bit like API documentation.) There are two ways to do this using dunder methods:



Iteration: __len__, __getitem__, __reversed__

In order to iterate over our account object I need to add some transactions. So first, I’ll define a simple method to add transactions. I’ll keep it simple because this is just setup code to explain dunder methods, and not a production-ready accounting system:

To iterate over transactions in reversed order you can implement the __reversed__ special method:


All in all, this account class is starting to look quite Pythonic to me now.
Operator Overloading for Comparing Accounts: __eq__, __lt__


This feels completely natural, but it’s actually quite amazing what happens behind the scenes here. Why does > work equally well on integers, strings and other objects (as long as they are the same type)? This polymorphic behavior is possible because these objects implement one or more comparison dunder methods.

An easy way to verify this is to use the dir() builtin:

>>> dir('a')
['__add__',
...
'__eq__',    <---------------
'__format__',
'__ge__',    <---------------
'__getattribute__',
'__getitem__',
'__getnewargs__',
'__gt__',    <---------------
...]





Note this works in both directions because we’re adding objects of the same type. In general, if you would add your object to a builtin (int, str, …) the __add__ method of the builtin wouldn’t know anything about your object. In that case you need to implement the reverse add method (__radd__) as well. You can see an example for that here.
Callable Python Objects: __call__

You can make an object callable like a regular function by adding the __call__ dunder method. For our account class we could print a nice report of all the transactions that make up its balance:



Please keep in mind that this is just a toy example. A “real” account class probably wouldn’t print to the console when you use the function call syntax on one of its instances. In general, the downside of having a __call__ method on your objects is that it can be hard to see what the purpose of calling the object is.

Most of the time it’s therefore better to add an explicit method to the class. In this case it probably would’ve been more transparent to have a separate Account.print_statement() method.
Context Manager Support and the With Statement: __enter__, __exit__





