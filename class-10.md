HOW TO DEAL WITH ERRORS



1: DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.
You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)
IE and Safari also have their own tools (but there is
not space to cover them all).



2: HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statement .Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.
In the latter part of the chapter, you will learn how to
gracefully check whether something will work, and
offer an alternative option if it fails

TRY, CATCH, FINALLY
This example displays JSON data
to the user. But, imagine that the
data is coming from a third party
and there have been occasional
problems with it that could
cause the page to fail.
This script checks if the JSON
can be parsed using a try block
before trying to di splay the
information to the users.
JAVASCRIPT
If the try statement throws an
error (because the data cannot
be parsed), the code in the catch
code block will be run, and the
error will not prevent the rest of
the script from being executed.
The catch statement creates
a message using the name and
message properties of the Error
object.
The error will be logged to the
console, and a friendly message
will be shown to the users of
the site. You cou ld also send
the error message to the server
using Ajax so that it could
be recorded. Either way, the
f i na 11 y statement adds a link
that allows users to refresh the
data they are seeing.
clO/