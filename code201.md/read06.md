**IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES**

If a variable is part of an object, it is called a
property. Properties tell us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.

**IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS**

If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.

**Programmers use a lot of name/value pairs:**

• HTML uses attribute names and values.

• CSS uses property names and values.

**In JavaScript:**

*• Variables have a name and you can assign them a
value of a string, number, or Boolean.*

*• Arrays have a name and a group of values. (Each
item in an array is a name/value pair because it
has an index number and a value.)*

*• Named functions have a name and value that is a
set of statements to run if the function is called.*

*• Objects consist of a set of name/value pairs
(but the names are referred to as keys).*

**The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas:**

*MAKING A MODEL OF THE
HTM L PAGE
When the browser loads a web page, it
creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.*


*ACCESSING AND CHANGING THE HTML PAGE
The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.*

# WORKING WITH THE DOM TREE

**Accessing and updating the DOM tree involves two steps:**

1: Locate the node that represents the element you want to work with.

2: Use its text content, child elements, and attributes.

----

**The terms elements and element nodes are used interchangeably
but when people say the DOM is working with an element,
it is actually working with a node that represents that element.**

**METHODS THAT RETURN A SINGLE ELEMENT NODE:**

getElementByld ( ' id ' )


Selects an individual element given the value of its i d attribute .

The HTML must have an id attribute in order for it to be selectable.

querySel ector( ' css selector ')

Uses CSS selector syntax that would select one or more elements .

This method returns only the first of the matching elements.

**METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):**

getEl ementsByClassName( ' class ' )

getEl ementsByTagName( ' tagName ')

querySelectorAll ( ' css select or ')

------

**LIVE & STATIC NODELISTS**

There are times when you will want to work with
the same selection of elements several times, so
the Nodelist can be stored in a variable and re-used
(rather than collecting the same elements again).
In a live Nodelist, when your script updates the
page, the Nodelist is updated at the same time.
The methods beginning getEl ementsBy_ return live
Node lists. They are also typically faster to generate
than static Nodelists.

# ADDING ELEMENTS USING DOM MANIPULATION

DOM manipulation offers another technique
to add new content to a page (rather than
i nnerHTML). It involves three steps:

1- *CREATE THE ELEMENT
createEl ement ()
You start by creating a new
element node using the
createElement() method.
This element node is stored
in a variable.
When the element node is
created, it is not yet part of the
DOM tree. It is not added to
the DOM tree until step 3.*

2- *GIVE IT CONTENT
createTextNode()
createTextNode() creates a new text node. Again, the node is stored in a variable. It can be added to the element node using the appendChi l d () method. This provides the content for the element, although you can skip this step if you want to attach an empty element to the DOM tree.*

3- *ADD IT TO THE DOM appendChild() Now that you have your element (optionally with some content in a text node), you can add it to the DOM tree using the appendChi 1 d () method. The appendChi 1 d () method allows you to specify which element you want this node added to, as a child of it.

----

# REMOVING ELEMENTS VIA DOM MANIPULATION

**DOM manipulation can be used to remove
elements from the DOM tree.**

*1- 
STORE THE ELEMENT
TO BE REMOVED IN A
VARIABLE
You start by selecting the
element that is going to be
removed and store that element
node in a variable.
You can use any of the methods
you saw in the section on DOM
queries to select the element.*

*2-
STORE THE PARENT OF
THAT ELEMENT IN A
VARIABLE
Next, you find the parent element
that contains the element you
want to remove and store that
element node in a variable.
The simplest way to get this
element is to use the parentNode
property of this element.*

*3- REMOVE THE ELEMENT
FROM ITS CONTA INING
ELEMENT
The removeChi ld() method is
used on the containing element
that you selected in step 2.
The removeChi ld() method
takes one parameter: the
reference to the element that
you no longer want.*

















