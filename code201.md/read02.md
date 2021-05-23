**When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.**

*● Structural markup: the elements that you can use to
describe both headings and paragraphs*

*● Semantic markup: which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on*

# Headings



h1 is used for main headings

h2  is used for subheadings If there are further sections
under the subheadings then the
 element is used, and so on ..


h3
h4
h5
h6

# Paragraphs

To create a paragraph, surround
the words that make up the
paragraph with an opening <p>
tag and closing </p> tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.

# Bold & Italic

b

By enclosing words in the tags
<b> and </b> we can make
characters appear bold.

i

By enclosing words in the tags
<i> and </i> we can make
characters appear italic.

# White Space

In order to make code easier to
read, web page authors often
add extra spaces or start some
elements on new lines.

-----
# css


**The key to understanding how CSS works is to
imagine that there is an invisible box around
every HTML element.**

*CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration*



CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.



h1, h2, h3 {

 font-family: Arial;

 color: yellow;

 }

 **Using Internal css**



You can also include CSS rules
within an HTML page by placing
them inside a style element,
which usually sits inside the
head element of the page


# javascript

*When you want to use JavaScript with a web page, you use the HTML script element to tell the browser it is coming across a script. Its s re attribute tells people where the JavaScript file is stored.*

----
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.

**COMMENTS**


You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code. 

**WHAT IS A VARIABLE?** 



A script w ill have to temporarily st ore the bits of info rmation it needs to do its j ob. It can store t his data in variables. 


**DATA TYPES** 

JavaScript distinguishes between numbers, strings, and true or false values known as Booleans. 


NUMERIC DATA TYPE The numeric data type handles numbers. 

STRING DATA TYPE The strings data t ype consists of letters and other characters. 

BOOLEAN DATA TYPE Boolean data types can have one of two values: true or false. 

**comparation opreators:**

!= is not equal to

== is equal to

=== strict equal to

!== strict not equal to

> greater than

< less than 

> greater or equal than

< less or equal than 