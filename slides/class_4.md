This page intentionally left blank. ⬇️, ➡️, or spacebar 🛰 to start slidedeck.
---
class: center, middle

# Welcome to Class 4!

---

# Agenda

- Questions from last week?
- News of the Week
- Readings
- Break!
- Introducing CSS
- BREAK!
- Introduction of Website Assignment
- LAB - working in groups


---
## Questions?

---

## News of the Week

Drop a link on the etherpad:
<https://etherpad.wikimedia.org/p/prattsi654fa20-4>

---
# Readings
- [What is code?](http://www.bloomberg.com/graphics/2015-paul-ford-what-is-code/)
- Everything else

---
# BREAK

.center[![](img/compacdisc.gif)]

---
# Cascading
# Style
# Sheets

.center[![](img/waterfall.gif)]

---
# Cascading

- (of water) pour downward rapidly and in large quantities.
- fall or hang in copious or luxuriant quantities.
- arrange (a number of devices or objects) in a series or sequence.


- Moment of zen: [Roadtrip Sunset](https://codepen.io/a-trost/details/pXzbbq)

.right[![](img/waterfall4.gif)]

---
# HTML is for structure, CSS is for design

- (demo on page)
- [CSS Zen Garden](http://www.csszengarden.com/)
- alternatively, [ashleyblewer.com](https://ashleyblewer.com)

---
# How to put CSS on the page

Something like this goes between your HTML `<head>` tags:

# `<link rel="stylesheet" href="style.css">`

---
# Applying CSS

- HTML elements
- HTML elements with a specific *class* attribute
- HTML elements with a specific *ID* attribute

---
# Basic syntax

```css
h1 {
	color: red;
}

.red {
	color: red;
}

#red {
	color: red;
}
```
---
# Basic syntax

```html
<h1>This header</h1>
<h1 class="red">This header</h1>
<h1 id="red">This header</h1>
```

---
# Basic syntax

```css
h1 {
	color: red;
}
```

- `h1` is the *selector*
- `{` and `}` hold the rules (called *declarations*)
- `color` is the property
- `red` is the value
- the semi-colon ends the declaration, and a new one can begin



---
# Multiple declarations

```css
h1 {
	color: red;
	font-weight: bold;
}
```

---
# Multiple selectors

```css
h1, h2 {
	color: red;
}
```

---
# Competing declarations

```css
h1 {
	color: red;
	color: pink;
}

h1 {
	color: blue;
}
```

---
# Children selectors

```css
#red > p {
	color: red
}
```

(Every paragraph tag nested inside of an element with an ID of "red")

---
# Sibling selectors

```css
h1 ~ p {
  color: red;	
}
```

(The paragraph tag that are at the same nested level as the h1 tag, and no others)

---
# Adjacent selectors

```css
h1 + p {
  color: red;	
}
```

(The paragraph tag that comes right after the h1 tag, and no others)

---
# HTML attributes with a certain value

```css
input[type=text] {
	border: 1px solid red;
}
```

(HTML forms that are text will have a red border)

---
# pseudo-elements

- h1::before
- h1::after

---
# psuedo-classes

- :checked
- :focus
- and more...

---
# `!important`

```css
h1 {
	color: red !important;
}

h1 {
	color: blue;
}
```

This is not really "good practice" but it's good in an emergency

---
# Comments in CSS

```css
/* this is a comment */
```

---
# Changing text

- `font-family` (serif, san serif, or names -- see next slide)
- `font-size` (make big or small -- see a few slides from now)
- `font-weight` (boldness or lack of)
- `font-style` (italic or lack of)
- `text-transform` (uppercase, lowercase, capitalize)

---
# Changing fonts

- Fonts are special; they are loaded from your computer
- Computers don't always have the same fonts
- Let's look at ["web-safe fonts"](https://www.cssfontstack.com/) 
- Fonts can also be embedded, using something like [Google fonts](https://fonts.google.com/)

---
# Changing fonts

- Here's how to do it: `h1 {font-family: "Open Sans", Verdana, sans serif;}`
- Note that you can "stack" fonts in this way
- The first is a two-word font name, the second is a font name on many computers, and the last is a general font style

---
# Sizing things

There are a lot of options:

- pixels (`width: 800px`)
- frames (`width: 1fr`)
- vertical width / vertical height (`width: 10vw`)
- percentage (`width: 80%`)

---
# Sizing text

- Em values (`4.2em`)
- pixels (`12px`)
- words (small, medium, large, xxx-large)
- points (pt), centimeters (cm), inches (in)

---
# Making space

- Everything on the web is a bunch of boxes even if it doesn't look like it
- padding (add space around element)
- border (add space around padding)
- margin (add space around border)

<div style="padding:40px;border: 20px solid black; margin:40px;">Box example</div>

---
# Lets talk about color

- 🌈🌈🌈
- Here's a list of the 140 named colors: [htmlcolorcodes.com](https://htmlcolorcodes.com/color-names/)
- "color" means changing the attribute's foreground color (e.g. text, border)
- `background-color` will change the color of the box area
---
# Color: lots of options

- `red`
- `rgb(255,0,0)`
- `rgb(100%,0%,0%)`
- `#ff0000`
- `#f00`
- `hsl(0,100,50)`

You can also add transparency to RGB or HSL values:
- `rgba(255,0,0,0.5)`
- `hsla(0,100,50, 0.5)`

---
# Native Frameworks

- [Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - native to CSS
- [Flexbox](https://css-tricks.com/snippets/css/complete-guide-grid/) - native to CSS

---
# Library Frameworks

- [Bootstrap](https://getbootstrap.com/) - classicccccccc, very popular, used in a lot of places
- [Materialize](https://materializecss.com/) - based on Google's design language
- [Pure.css](https://purecss.io/) - basic and easy to learn
- [Tufte.css](https://edwardtufte.github.io/tufte-css/) - make your page look like Edward Tufte books 
- ... and so many more!

---
# CSS for page layouts

<iframe width="560" height="315" src="https://www.youtube.com/embed/KOvGeFUHAC0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

- [Fast Layouts with CSS Grid](https://www.youtube.com/watch?v=KOvGeFUHAC0)

---
# Grid resources 

- [CSS Grid Garden](https://cssgridgarden.com/)
- [CSS Tricks: A complete guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---
# Flexbox resources

- [CSS Tricks: A complete guide to Flexbox](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Flexbox Defense](http://www.flexboxdefense.com/)

---
# Remember CSS is always changing

<iframe width="560" height="315" src="https://www.youtube.com/embed/sZS-7RX_c7g" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

- [New CSS for Styling Underlines on the Web](https://www.youtube.com/watch?v=sZS-7RX_c7g)

---
# Advanced: CSS 3D, transformations and animations

- [Unfolding the Box Model](https://rupl.github.io/unfold/) (Examples of appearing 3D)
- [CSS 3D Clouds](https://www.clicktorelease.com/code/css3dclouds/)

---
# Additional resources

- [The CSS Saga](http://www.w3.org/Style/LieBos2e/history/Overview.html)
- [Code.org: Web Development: Intro to CSS](https://www.youtube.com/watch?v=EP9QMdoXvXE) (video)
- Rachel Andrews. [The W3C at Twenty-Five](https://www.smashingmagazine.com/2019/10/happy-birthday-w3c/)
- [Old CSS, New CSS](https://eev.ee/blog/2020/02/01/old-css-new-css/)

Technical resources:
- [CSS Basics](http://www.cssbasics.com/)
- [Mozilla: Introduction to CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS)
- [Mozilla: CSS Selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Selectors)
- [HTML Dog: CSS Beginner Tutorial](https://www.htmldog.com/guides/css/beginner/)

Bonus:
- [How to Center in CSS](http://howtocenterincss.com/) (Because it will definitely come up!)
- Jennifer Dewalt. [180 websites in 180 days](https://jenniferdewalt.com/) ([Background talk on this project](https://www.youtube.com/watch?v=QaSbL4sRff8))

---
# BREAK

---
# Personal Homepage project

- Assignment details [here](https://github.com/hadro/info654fa20/blob/master/assignments/personal_homepage.md)
- Questions?

---
# Breaking into groups

- We are going to use the Breakout Rooms feature of Zoom to split everyone into small groups
- Start working on your assignments and ask each other questions
- Ashley and Josh will "walk around the room", dropping into each Zoom room to answer questions and offer help
