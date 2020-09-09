This page intentionally left blank. ⬇️, ➡️, or spacebar 🛰 to start slidedeck.
---
class: center, middle

# Welcome to Class 3!

---

# Agenda

- Questions from last week?
- News of the Week
- Imperfect metaphor of the week
- Readings
- Break!
- Viewing Code
- Document Structure
- Basic HTML elements
	 - Elements vs. Attributes
- BREAK!
- Validating Code
- Working with HTML


---

## Assignment questions?

### Other questions?

---

## News of the Week

Drop a link on the etherpad:
<https://etherpad.wikimedia.org/p/prattsi654fa20-3>

---
class: center, middle

#Imperfect metaphor of the week
---
background-image: url(https://www.barnesandnoble.com/blog/sci-fi-fantasy/wp-content/nas-uploads/sites/4/2019/09/matrix.png)

---

<https://web.archive.org/web/20120313124550/http://labs.syropia.net/MatrixText/>

(View in Chrome)

---

# Readings

What main take-aways did you get from these?

What questions do you have?


---
class: center, middle

# World Wide Web Review

.center[![](./img/bgstar.gif)]

---
# First website

.center[![](./img/cernsite-now.jpg)]

- [see for yourself](http://info.cern.ch/hypertext/WWW/TheProject.html)

---
# Another important website

.center[![](./img/spacejam-now.jpg)]

- [see for yourself](https://www.spacejam.com/)

---
# Technologies

Important technologies that make up the web:

- hypertext
- domain name system
- browsers

---
# Hypertext

- inspired by the "memex" concept
- jumping from text to text, creating links
- WWW brought hypertext to a global scale

---
# History of Hypertext

- See: Vannevar Bush's [As We May Think](https://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/?single_page=true) (1945)
- See: Douglas Engelbart and Team's [Mother of All Demos](https://www.youtube.com/watch?v=B6rKUf9DWRI) (1968)
- See: Apple Macintosh's [HyperCard](https://en.wikipedia.org/wiki/HyperCard)

(Don't miss archived HyperCard collections on Archive.org, e.g. <https://archive.org/details/hypercard_twin-peaks>)


---
# HTTP(S)

What is this?

.center[![](./img/sparklewhite.gif)]

---
# HTTP(S)

## Hyper
## Text
## Transfer
## Protocol
## (Secure)

---
# Distributed Name Service (DNS)

- Think back to last week -- what does this do?

.center[![](./img/dnsbutton.gif)]

---
# Browsers and more


.center[![under-construction](./img/under-construction.gif)]

--

What are the browsers you are familiar with?

Which ones do you use every day?

--

What's the earliest browser you have memories of?


---

##  Blast from the past: [Lynx](https://en.wikipedia.org/wiki/Lynx_(web_browser) (1992 - )

"the oldest web browser still in general use and active development"

![](./img/lynx.png)

(View of our syllabus on Github via Lynx browser)


---
# Additional Resources

- [Broad Band: The Untold Story of the Women Who Made the Internet by Claire L. Evans](https://www.goodreads.com/book/show/35953464-broad-band)
- [ How the Internet Happened: From Netscape to the iPhone by Brian McCullough](https://www.goodreads.com/book/show/38212134-how-the-internet-happened)
- [Project Code Rush - The Beginnings of Netscape](https://www.youtube.com/watch?v=4Q7FTjhvZ7Y)

---
# HTML

.center[![](./img/spingreenguy.gif)]

---
# HTML

- Needed to convey information over the internet
- neutral way of writing that can be read by any application
- based on SGML (Standard Generalized Mark-up Language)
- a sibling to XML (eXtensible Mark-up Language)
  - Essentially, a stricter subset of possible XML markups
- was created for sharing documents

(Fun fact from your readings: since HTML was designed for sharing 1980s physics papers, whether to include images or not was hotly debated. Can you fathom a WWW without pictures of cats?)

---

# HTML

Separating **Document Structure** from *Style*

--

Why is this necessary? Why develop it this way?

--

(A way to visualize this: In Firefox, you can easily turn off styles for any web page. Go to "View" -> "Page Style" -> "No Style" -- just remember to toggle it back when you're done!)

---

# HTML5

- Like all languages, HTML has changed over time
- Some things go away:
  - `<blink></blink>`
  - `<marquee></marquee>`
- Another example of the web changing: [Seasonal Restoration](https://blog.geocities.institute/archives/6620)
- Many new attributes are added to make the web easier to view
- expanded to handle more than just documents


---

# before we dive in

--

## Let's look at code

---

Because the Web is built on open standards...

All the source code is there for you to view!

Your new best friend: "View Source"

### Chrome
View -> Developer -> View Source

### Firefox
Tools -> Web Developer -> Page Source

<https://neilpatel.com/blog/how-to-read-source-code/>

---

## Spend a minute looking at code!

![](https://www.barnesandnoble.com/blog/sci-fi-fantasy/wp-content/nas-uploads/sites/4/2019/09/matrix.png)

Find a page you visit frequently, and use the "view source" tool to look at the underlying HTML.

What do you notice? Do you see anything interesting?

---

# Document Object Model (DOM)

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1024px-DOM-model.svg.png" style="height: 500px" />

---

# Other views

<img src="https://www.jaimebutler.ch/jb-edit/wp-content/uploads/2014/07/Basic-HTML.png" style="height: 500px" />

---

# Other views

![](https://help.madcapsoftware.com/flare2017r3/Content/Resources/Images/Flare/page_structure_example.png)

---

# What is an 'element'?

Two options, both in meta-code:

**`<element attribute="value"> content that the element wraps around</element> `**

(more common)

or

**`<element attribute="value"> `**

(Less common, called a self-closing tag or element)

---

# Let's learn some real HTML elements

```html
<!DOCTYPE html>
<html>
    <head>
	    <title></title>
    </head>
    <body>
	    <h1>My page</h1>
    </body>
</html>
```

---
# HTML

## `<html></html>`

- holds everything together
- The "spine" of all nested elements

---
# Head and Body

## `<head></head>`
## `<body></body>`

---
# Head

```html
<head>
	<title>Information in your browser tab</title>
	<meta charset="utf-8">
	<link rel="stylesheet" type="text/css"
      href="//fonts.googleapis.com/css?family=Open+Sans" />
</head>
```
---
# Body

```html
<body>
	<h1>Everything you see on the page</h1>
	<p>Everything you see on the page will go in the body of the HTML</p>
</body>
```

---
# Heading tags

```html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

--
# An `h1` heading
## An `h2` heading
### An `h3` heading
#### An `h4` heading
etc.


---
# HTML5 Semantic elements

```html
<header></header>
<nav></nav>
<aside></aside>
<footer></footer>
```
... and [more](https://guide.freecodecamp.org/html/html5-semantic-elements/)

---
# Tables
(spreadsheets on the web)

<table style="border:4px solid black;font-size:1.4em;">
  <tr>
    <td style="border:4px solid darksalmon">Row 1, column 1</td>
    <td style="border:4px solid darksalmon">Row 1, column 2</td>
    <td style="border:4px solid darksalmon">Row 1, column 3</td>
  </tr>
  <tr>
    <td style="border:4px solid green">Row 2, column 1</td>
    <td style="border:4px solid green">Row 2, column 2</td>
    <td style="border:4px solid green">Row 2, column 3</td>
  </tr>
</table>

---
# Tables

```html
<table>
  <tr>
    <td>Row 1, column 1</td>
    <td>Row 1, column 2</td>
    <td>Row 1, column 3</td>
  </tr>
  <tr>
    <td>Row 2, column 1</td>
    <td>Row 2, column 2</td>
    <td>Row 2, column 3</td>
  </tr>
</table>
```

- [Mozilla web docs: Tables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

---
# Lists

```html
<ul>
	<li>List item in an unordered list</li>
	<li>Another list item</li>
</ul>
<ol>
	<li>List item in an ordered list</li>
	<li>List item 2</li>
</ol>
```

---
# Lists, rendered

<ul>
	<li>List item in an unordered list</li>
	<li>Another list item</li>
</ul>
<ol>
	<li>List item in an ordered list</li>
	<li>List item 2</li>
</ol>

---
# Comments

## `<!-- This is an HTML comment -->`

When this appears in the code, anything between the `<!--` and the next `-->` won't actually get rendered by the browser (it stays in the code).

(For one example, the ASCII art in the code underlying the Tumblr homepage is hidden an HTML comment just like this; see <https://www.tumblr.com/>)


---
# Elements and Attributes

- Everything we just covered were HTML **elements**
- Elements can have **attributes**
- Attributes are "key-value pairs" that fit inside HTML elements
- Attributes are what make the Web work! It's what Vannevar Bush got super excited about, the "mesh of associative trails"
- The next few pages are examples

---
# Linking

### `<a href="http://training.ashleyblewer.com">Link text</a>`

- `a` is the HTML element
- `href` is the attribute
- the website is the value of the attribute

--

# The markup above rendered:

### <a href="http://training.ashleyblewer.com">Link text</a>

---
# Embedding images

## `<img src="/img/greenguy.gif">`

- `img` is the HTML element
- `src` ("source") is the attribute
- the path to where the image is is `src`'s value
- Note that this is an example of one of the few "self-closing" elements

---
# Embedded images and ALT text

`<img src="/img/greenguy.gif" alt="rotating alien">`

- `alt` is the HTML attribute for images that provide screenreaders with a brief decsription of the word, or show up when the image itself cannot load

---
Here's an example of what that looks like:


With a broken URL: <img src="./img/intentionallybadlink.gif" alt="rotating alien" title="rotating alien" />

With a good URL: <img src="./img/spingreenguy.gif" alt="rotating alien" title="rotating alien" />

---
# What about that DOCTYPE?

`<!DOCTYPE html>`

- "document type declaration"
- lets the computer know what kind of file this is, even though your browser can probably guess

---
# ...and more!

There are many more elements and aspects to HTML than covered here; this is just an overview of some of the major concepts.

---
class: middle

.center[ # [Validate, validate, validate](https://validator.w3.org/)]

---
# Things to remember

- Most HTML elements need an "opening" and "closing" tags.
- The exception to this is if they are "self-closing" (for elements that don't need any text content in between, like `img` or `br`)

---
# Cheat sheets

Use these to help remember syntax and rules!

- [HTMLCheatSheet.com](https://htmlcheatsheet.com/)
- [Stanford HTML Cheatsheet](https://web.stanford.edu/group/csp/cs21/htmlcheatsheet.pdf) (PDF)

---

# HTML exercise

There are great tools out there that let you write HTML and see in real-time what it looks like.

One we like is called <https://repl.it/> (works with many programming languages)

(Glitch is another popular one, with similar functionality: <https://glitch.com/>)

---

# HTML exercise

Remember the first webpage ever?

--

Here's the URL: <http://info.cern.ch/hypertext/WWW/TheProject.html>

Funny enough, the HTML on that page is actually no longer valid!

As a quick exercise, using the <Repl.it> tool from the previous slide, try using the following elements to recreate the first few lines of that web page in current valid html:
- H1: `<h1>Heading here</h1>`
- Paragraph: `<p>Paragraph text here.</p>`
- Anchor: `<a href="URL_here">Link text</a>`

---
# Additional resources

- [Mozilla web docs: Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)
- [Definition Lists vs Tables (for accessibility)](https://snook.ca/archives/html_and_css/definition-lists-v-tables)
