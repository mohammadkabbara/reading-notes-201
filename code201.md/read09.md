# Why Forms?


The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.

# How Forms Work

1- A user fills in a form and then presses a button
to submit the information to the server.

2-The name of each form
control is sent to the
server along with the
value the user enters or
selects.

3-The server processes
the information using a
programming language
such as PHP, C#, VB.net,
or Java. It may also store
the information in a
database.

4-The server creates a new
page to send back to the
browser based on the
information received.

# HTML5: Form Validation

You have probably seen forms
on the web that give users
messages if the form control has
not been filled in correctly;

 this is
known as form validation.
Traditionally, form validation
has been performed using
JavaScript (which is beyond the
scope of this book). 

But HTML5
is introducing validation and
leaving the work to the browser.
Validation helps ensure the
user enters information in a
form that the server will be able
to understand when the form
is submitted. Validating the
contents of the form before it is
sent to the server the helps:

**● Reduce the amount of work
the server has to do**

**● Enables users to see if there
are problems with the form
faster than if validation were
performed on the server.**

# List Shorthand

As with several of the other CSS
properties, there is a property
that acts as a shorthand for list
styles. It is called list-style,
and it allows you to express
the markers' style, image and
position properties in any order

# table Properties

You have already met several
properties that are commonly
used with tables. Here we will
put them together in a single
example using the following:

**width** 

to set the width of the
table

**padding** 

to set the space
between the border of each table
cell and its content

**text-transform**

 to convert the
content of the table headers to
uppercase

**letter-spacing, font-size**


to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers

**text-align**

 to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows

**:hover**

 to highlight a table row
when a user's mouse goes over it Here are some tips for styling
tables to ensure they are clean


#  styling Submit Buttons

Here are some properties that
can be used to style submit
buttons. This example builds
on the one in the previous page,
and the submit button inherits
the styles set for the <input
element on the last page

**color**

 is used to change the
color of the text on the button.
**text-shadow**

 can give a 3D
look to the text in browsers that
support this property.

**border-bottom**

 has been used
to make the bottom border of
the button slightly thicker, which
gives it a more 3D feel.

**background-color**

 can make
the submit button stand out
from other items around it.
(Creating a consistent style
for all buttons helps users
understand how they should
interact with the site.) A gradient
background has been added for
browsers that support gradients.

**The :hover** 

pseudo-class
has been used to change the
appearance of the button when
the user hovers over it. In this
case, the background changes,
the text gets darker, and the
thicker border is applied to the
top of the button.

# HOW EVENTS TRIGGER JAVASCRIPT CODE

1-Select t he element
node(s) you want the
script to respond to.
For example, if you want to
trigger a function when a user
clicks on a specific link, you need
to get the DOM node for that
link element. You do this using a
DOM query 

2-Indicate which event on
the selected node(s) will
trigger the response.
Programmers call this binding an
event to a DOM node.

3-State the code you want
to run when the event
occurs.
W hen the event occurs, on a
specified element, it will trigger
a function. This may be a named
or an anonymous function.

---------


**Here you can see how event handling can be used to provide feedback to
users filling in a registration form. It will show an error message if their
username is too short.**



**SELECT ELEMENT**

The element that users are
interacting with is the text input
where they enter the username.

**SPECEFY EVENT**

When users move out of the
text input, it loses focus, and the
blur event fires on this element.

**CALL CODE**

When the blur event fires
on the username input, it
will trigger a function called
chec kUsername ().This function
checks if the username is less
than 5 characters.





