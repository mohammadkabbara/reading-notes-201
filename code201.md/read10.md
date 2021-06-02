# ORDER OF EXECUTION

**To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run:**

1. The greeting variable gets its value from the
greetUser() function.

2. greetUser() creates the message by combining
the string 'He 11 o ' with the result of getName ().

3. getName () returns the name to greetUser().

# EXECUTION CONTEXTS

**The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.**

EXECUTION CONTEXT


Every statement in a script lives in one of three
execution contexts:

*Q GLOBAL CONTEXT*
Code that is in the script, but not in a function.
There is only one global context in any page.

*FUNCTION CONTEXT*
Code that is being run within a function.
Each function has its own function context.

*Q EVAL CONTEXT (NOT SHOWN)*
Text is executed like code in an internal function
called eva l {) (which is not covered in this book).

VARIABLE SCOPE

The first two execution contexts correspond with the
notion of scope :

*Q GLOBAL SCOPE*

If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.

*FUNCTION-LEVEL SCOPE*

When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope.

# UNDERSTANDING SCOPE

In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object.

# UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code.

# ERROR OBJECTS

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.

# HOW TO DEAL WITH ERRORS

there are two things you can do with the errors.

**1: DEBUG THE SCRIPT TO FIX ERRORS**

If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.

You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)

IE and Safari also have their own tools.

**2: HANDLE ERRORS GRACEFULLY**
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statements.

Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.


In the latter part of the chapter, you will learn how to
gracefully check whether something will work, and
offer an alternative option if it fails.





