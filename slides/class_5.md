This page intentionally left blank. ⬇️, ➡️, or spacebar 🛰 to start slidedeck.
---
class: center, middle

# Welcome to Class 5!

---

# Agenda

- Questions from last week?
- News of the Week
- Readings
- Break!
- Web wrap-up
- Files, files, files!
- BREAK!
- Website project breakout groups



---

## Assignment questions?

### Other questions?

---

## News of the Week

Drop a link on the etherpad:
<https://etherpad.wikimedia.org/p/prattsi654fa20-5>

---

# Readings

- I have slides for these
- Let's step through each of them and discuss
---
# Readings -- some notes

- Cobweb
  - we will talk about this topic more in future classes
  - [bellingcat](https://www.bellingcat.com/)
  - [Internet Archive's Wayback Machine](https://web.archive.org/)
  - [perma.cc](https://perma.cc/)
  - version control
  - robots.txt
  - (Internet Archive has [changed its mind](https://blog.archive.org/2017/04/17/robots-txt-meant-for-search-engines-dont-work-well-for-web-archives/) about that)
  - web archiving -- more next week

---
# Readings -- some notes

## Bodleian and UCLA
  - digitization
  - as an example: NYPL has a photo team of around 12 people
  - [IIIF](https://iiif.io)... (Josh)
  - [Laurie Spiegal](https://en.wikipedia.org/wiki/Laurie_Spiegel)
  - [Part 1](https://youtu.be/TzOJtZYsGSA?t=226) - explaining digital vs analog
  - [Part 2](https://www.youtube.com/watch?v=oconRQBZff0) - "how does the computer help you save time?"
  - a lot of technical jargon: Aja, Blackmagic, XLR, TBC, etc
  - workflow diagrams!
  - reliance on software by companies

---
# Readings -- some notes

 - Let's step by step through the [h264 article](https://sidbala.com/h-264-is-magic/)
 - and the [JPEG playground article](https://parametric.press/issue-01/unraveling-the-jpeg/) -- again with the standards!
 - Amy Wibowo comes up again -- [Glitching hour](https://www.thestrangeloop.com/2018/the-glitching-hour.html) toy
 - rgb vs YCbCr, how do our eyes work?


---
class: center, middle

# Web wrap-up

- JavaScript, the missing puzzle piece
- What questions do you have about web tech?

---
# Compression

  - images, video, and audio, text
  - Compacting of bits in order to streamline file size
  - can see it on the web, like a bootstrap.min.js file
  - can see it when images look bad

---

 ![pixel loss](https://upload.wikimedia.org/wikipedia/commons/e/e9/Felis_silvestris_silvestris_small_gradual_decrease_of_quality.png)

---
# Generation loss

<iframe width="560" height="315" src="https://www.youtube.com/embed/DYvNsiJwldg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
class: middle

# .center[💻 File Formats 💻]

---
# Let's talk about files

- What is a file?
- What is a file format?
- Magic numbers
- File structures
- Standardization
- Registries

---
# Files

Things that can be
- Open
- Read 
- Changed
- Closed
- Permissions modified

---
# File Formats

We have many different types of files! These are categorized into different formats, with different ways to determine what to do with the data inside the file.

---
# Magic numbers

What separates a file from the rest of the binary landscape?
### Magic numbers!
Magic numbers are sometimes known as file signatures. They are a short string of hexadecimal code that  allow a file to identify itself as a certain type of file.

---
# File structure

- Magic numbers (file signature)
- Header
- Body (or payload)

---
# File standardization

- Outlines all the rules required to follow to have a valid file
- Can be standardized through a standards body (but not required)
- Can be open (anyone can read) or closed (proprietary, only people in a company/organization can access)

---
# Standardization example

A great resource for explaining how a file format is made, by Ross Spencer:
[http://exponentialdecay.co.uk/blog/genesis-of-a-file-format/](http://exponentialdecay.co.uk/blog/genesis-of-a-file-format/)

---
# Learning about file formats

- [ArchiveTeam's File Format Wiki](http://fileformats.archiveteam.org)

---
# Registries 

- [PRONOM](http://www.nationalarchives.gov.uk/PRONOM/Default.aspx) (UK National Archives)
- [Format Descriptions](https://www.loc.gov/preservation/digital/formats/fdd/browse_list.shtml) (US Library of Congress)
- [`file`](https://en.wikipedia.org/wiki/File_(command)) (Unix command)
- [File Formats Wiki](http://fileformats.archiveteam.org/wiki/Main_Page) (ArchiveTeam)

---
# Images

## JPEG
- came around in the 90s, varying degrees of Compression, very popular

## GIF
- pronounce as you like, not good quality but it can loop
- have become videos now on the web, including giphy.com!

## PNG
- lossless compression, which means its bigger. not very web-optimized but higher quality.
- it also has another layer, transparency!

---
# Images, cont

## SVG
- XML for images (like we saw on the nytimes homepage)
- this is vector-based instead of pixel-based
- Illustrator instead of Photoshop 
- we can view source on this https://www.w3.org/html/logo/downloads/HTML5_Logo.svg
- raster vs vector https://upload.wikimedia.org/wikipedia/commons/6/6b/Bitmap_VS_SVG.svg

## Other formats...
- BMP, TIFF, JPEG2000, RAW

---

## Audio

- WAV (regular, LPCM, BWF)
- limited to 4GB, very high quality stream though
- FLAC

## Video
- containers and codecs (same for audio)

---
class: middle, center

# Questions?

---
# Breakout groups