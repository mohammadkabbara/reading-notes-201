**Building Blocks**

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

**Containing Elements**

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

# Controlling the Position of Elements

**Normal flow**

Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside, they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).

**Relative Positioning**

This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

**Absolute positioning**

This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.

**Fixed Positioning**

This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.

**Floating Elements**

Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.

# Floating Element

The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.
Anything else that sits inside
the containing element will
flow around the element that is
floated


# CSS Frameworks

CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.

**ADVANTAGES**

● They save you from
repeatedly writing code for
the same tasks.

● They will have been tested
across different browser
versions (which helps avoid
browser bugs)

**DISADVANTAGES**

● They often require that you
use class names in your
HTML code that only control
the presentation of the page
(rather than describe its
content).


*● In order to satisfy a wide
variety of needs, they often
contain more code than you
need for your particular web
page (commonly referred to
as code “bloat”).*


# Liquid Layouts

**Advantages**

● Pages expand to fill the entire
browser window so there are
no spaces around the page
on a large screen.

● If the user has a small
window, the page can
contract to fit it without the
user having to scroll to the
side.

● The design is tolerant of
users setting font sizes larger
than the designer intended
(because the page can
stretch).

**Disadvantages**

● If you do not control the
width of sections of the page
then the design can look very
different than you intended,
with unexpected gaps around
certain elements or items
squashed together.

● If the user has a wide
window, lines of text can
become very long, which
makes them harder to read.

● If the user has a very narrow
window, words may be
squashed and you can end up
with few words on each line.

● If a fixed width item (such as
an image) is in a box that is
too small to hold it (because
the user has made the
window smaller) the image
can overflow over the text.

