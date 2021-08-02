# Introduction

List comprehensions offer a succinct way to create lists based on existing lists. When using list comprehensions, lists can be built by leveraging any iterable, including strings and tuples.

Syntactically, list comprehensions consist of an iterable containing an expression followed by a for clause. This can be followed by additional for or if clauses, so familiarity with for loops and conditional statements will help you understand list comprehensions better.

List comprehensions provide an alternative syntax to creating lists and other sequential data types. While other methods of iteration, such as for loops, can also be used to create lists, list comprehensions may be preferred because they can limit the number of lines used in your program.
List Comprehensions

In Python, list comprehensions are constructed like so:

list_variable = [x for x in iterable]

 
A list, or other iterable, is assigned to a variable. Additional variables that stand for items within the iterable are constructed around a for clause. The in keyword is used as it is in for loops, to iterate over the iterable.

Let’s look at an example that creates a list based on a string:

shark_letters = [letter for letter in 'shark']
print(shark_letters)

 

Here, the new list is assigned to the variable shark_letters, and letter is used to stand in for the items contained in the iterable string 'shark'.

For us to confirm what the new list shark_letters looks like, we call for it to print() and receive the following output:

Output
['s', 'h', 'a', 'r', 'k']

The list we created with the list comprehension is comprised of the items in the string 'shark', that is, one string for each letter.

List comprehensions can be rewritten as for loops, though not every for loop is able to be rewritten as a list comprehension.

Using our list comprehension that created the shark_letters list above, let’s rewrite it as a for loop. This may help us better understand how the list comprehension works.