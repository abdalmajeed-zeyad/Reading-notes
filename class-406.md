
How to use the Random Module in Python

 

In this post, I would like to describe the usage of the random module in Python. The random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.
When to use it?

We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.
Random functions

The Random module contains some very useful functions.
Randint

If we wanted a random integer, we can use the randint function Randint accepts two parameters: a lowest and a highest number. Generate integers between 1,5. The first value should be less than the second.

import random
print random.randint(0, 5)

This will output either 1, 2, 3, 4 or 5.
