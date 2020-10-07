This page intentionally left blank. ⬇️, ➡️, or spacebar 🛰 to start slidedeck.
---
class: center, middle

# Welcome to Class 7!

---

# Agenda

- Questions?
- News of the Week
- Readings
- Break!
- Structured Data
- XML
- JSON


---

## Assignment questions?

### Other questions?

---

## News of the Week

Drop a link on the etherpad:
<https://etherpad.wikimedia.org/p/prattsi654fa20-7>

---
class: middle, center

# Break!

---
# Imperfect Metaphor of the Week

https://www.flickr.com/search/?q=scaffolding%20gaudi

---

# What is structured data?

--

## What are examples of unstructured data?

--

## What are examples of structured data?


---

# XML

---
# XML

XML is a means of sharing data between computers. It can be read and understood
by humans, but its primary purpose is to be a way of exchanging information
between computers or systems.

By doing this in a structured, standardized way, it allows for data to be
passed from one system to the other without any ambiguity.

If you think of the game "Telephone" where people pass a message between each
other through whispering, it is easy to have that original message distorted
somewhere along the way. XML is a way to prevent data distortion.


---
# Three markup-related things we've seen so far this semester

- XML
- HTML
- XHTML

--

## What's the connection among these things?


---

Before we dive into the details of XML...
--

## What do you think are some important ways HTML and XML differ?


---
# XML

XML is a relative of HTML

- XML is **extensible**: it does not consist of a fixed (limited) set of tags
- XML must be **well-formed** according to a defined specification
- XML documents can be **validated** against a specific schema (not just one global schema)
- XML is about the data (its contents) and not about how that data is presented

---
# XML structure

- XML must have a **declaration**
- XML can have **namespaces**
- XML has **elements**
- XML can have **attributes**

---
# Namespaces

.center[![](./img/ns.png)]

---
# Document declaration

`
<?xml version="1.0" ?>`

This is to let the software reading an XML file that you are going to present it
with XML. Computers don't always trust the file extension or other indicators
that a document is what it says it is. This says "I have prepared this XML, and
this declaration at the top of the file lets you know that XML is coming through
next."

---
# Simple Example

```
<?xml version="1.0" ?>
<books>
<book>
<title>My Father's Dragon</title>
<author>Ruth Stiles Gannett</author>
<subjects>
<subject>Children's</subject>
</subjects>
</book>
</books>
```

---
# Example with attributes

```
<movies>
<movie id="3">
<title language="french">Jeanne Dielman, 23, Quai du Commerce, 1080 Bruxelles</title>
<director nationality="belgian">Chantal Akerman</director>
</movie>
</movies>
```

---
# How to expand?

```
<?xml version="1.0" ?>
<books>
<book>
<title>My Father's Dragon</title>
<author>Ruth Stiles Gannett</author>
<subjects>
<subject>Children's</subject>
</subjects>
</book>
</books>
```

---
# Simple Example

```
<?xml version="1.0" ?>
<books>
<book>
<title lang="en">My Father's Dragon</title>
<title lang="es">El Dragon de papa</title>
<title lang="jp">エルマーの冒険</title>
<people>
<author>Ruth Stiles Gannett</author>
<illustrator>Ruth Chrisman Gannett</illustrator>
</people>
...
</book>
</books>
```
---
## Let's look at a live example

--

## Simple Example

From the US Senate, which has been publishing XML for decades:

https://www.senate.gov/legislative/LIS_MEMBER/cvc_member_data.xml

(You may have to do "view source" to see the XML correctly)

---
## More complex example

Semantic markup of the Abraham Lincoln Papers collection, held by the Library of Congress:

https://findingaids.loc.gov/exist_collections/ead3master/mss/2009/ms009304.xml

(You may have to do "view source" to see the XML correctly)

---

# XML has rules

You must follow these rules when you create XML syntax:

- All XML elements must have a closing tag.
- XML tags are case sensitive.
- All XML elements must be properly nested.
- All XML documents must have a root element.
- Attribute values must always be quoted.

---
# All XML elements must have a closing tag

Not OK:
```
<books
<book></book>
</books>
```

---
# XML tags are case sensitive

Not OK:
```
<Books>
<book>
</book>
</books>
```

---
# All XML elements must be properly nested.

Not OK:
```
<books>
<book>
</books>
</book>
```

---
# All XML documents must have a root element

Not OK:
```
<?xml version="1.0" ?>
<books></books>
<books></books>
<books></books>
```
---
# Attribute values must always be quoted


Not OK:
```
<books>
<book id=num123>
</book>
</books>
```

---
# What if I want to use characters that are already being used?

You will have to "escape" them by using other characters that are designed to
represent what you want. Some examples:

- type <code>& amp ;</code> to display the `&` character
- type <code>& lt ;</code> to display the `<` character
- type <code>& gt ;</code> to display the `>` character
- type <code>& quot ;</code> to display the `"` character
- type <code>& apos ;</code> to display the `'` character

(Without spaces, and including the semicolon!)
---
# Where else can you find XML?

XML as a way to exchange data is the foundation of several well-known file
formats:

- SVG files
- PDF files
- Microsoft Office files (.docx, .xlsx, and .pptx)

---
# A note on validation

XML can be validated against its specification, to make sure it is well-formed
structured data, with no errors like described above.

But XML can also be validated against other XML files known as XSD.

XSD stands for XML Schema Definition.

These XSD
files describe the intended structure of a document -- so not only checking to
see if the metadata is well-formed, but if it adheres to more rigid standards
like the expectation of specific fields or attributes, or in a specific order.

---
# Also, DTDs

DTD stands for "Document type definition". It is another way to define a desired
XML structure, but the syntax is different from XML itself (although similar, I
guess).

A `DTD` can be seen at the top of every valid HTML page:

`<!DOCTYPE html>`

Note this is different from the XML declaration (`<?xml version="1.0"
encoding="utf-8"?>`) at the top of XML documents, and note how the structure is different.

---
# Additional Resources

- [Getting started with XML: A workshop](http://infomotions.com/musings/getting-started/getting-started.pdf)
- [xmllint](https://linux.die.net/man/1/xmllint)


---

# JSON

---
# JSON

- "JavaScript Object Notation"
- a way to exchange informations (computers talking to computers)
- a standard, which means it has a [written specification](https://www.json.org/json-en.html) and rules for how it works.
- related to javascript but doesn't have to be used only with javascript

---
# Example

```
{
  "firstName": "Ashley",
  "lastName": "Blewer",
  "isAlive": true,
  "age": 100,
  "address": {
    "streetAddress": "123 Main Street",
    "city": "New York",
    "state": "NY",
    "postalCode": "11111"
  },
  "phoneNumbers": [
    {
      "type": "home",
      "number": "555 555-1234"
    },
    {
      "type": "mobile",
      "number": "123 456-7890"
    }
  ]
}
```

---
# Data types

- numbers (e.g. 1)
- strings (e.g. "Hello")
- booleans (e.g. `true`)
- no value (e.g. `null`)

---
# Data structures

- elements in curly braces! (`{` and `}`)
- arrays (things inside of `[` and `]`)
- objects ("key": "value" pairs)

---
# Other bits to notice

- String literals (e.g. "\"Phrase in Double Quotes, inside of Quotes\"")
- Quotation marks = strings
- Booleans are not wrapped in quotation marks
- Elements can repeat but you must use a comma

`{ "a":123, "b":[1,2,3], "c": { "a":1, "b":2 } }`


---

# Exercise time

Two options:

1. Work with Senate data in xml
2. Try an XML to JSON conversion

---
##Option 1

- Pick a senate race that is likely to [flip a senate senate](https://projects.fivethirtyeight.com/2020-election-forecast/senate/) [Iowa (IA) and Maine (ME) are two good options...]
- Using the [Senate contacts XML](https://www.senate.gov/general/contact_information/senators_cfm.xml), see how close you can get to generating the right XML for the new senator if the seat does flip
  - What data are you missing?
  - What other data would be interesting to include in the XML?

## Option 2
- Pick a US Senator from the [Senate committee assignments xml](https://www.senate.gov/legislative/LIS_MEMBER/cvc_member_data.xml)
- Try modeling a single `<senator>` example from that list as JSON.
  - How does nesting work in JSON?
  - How do you translate XML attributes into JSON?
- Try using a JSON validator to make sure the JSON is legal ([option 1](https://jsonlint.com/?code=), [option 2](https://jsonformatter.curiousconcept.com/))
