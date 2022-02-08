# A tutorial/key for html
Made as i was learning it myself

# Introduction

Everything in html starts with a <> with a value inside, and most the time ends with a </> with a value after the /\

**Span** = inline/short pieces of text, **div** = block\
These are useful for mantainability, and assigning id's/classes.\
They're not necessary but seperate code into multiple blocks which are easier to read\

Use a **class** for something that'll appear multiple times, **id** for something thatll appear once

# The Basics

General
- Paragraphs = ``<p> </p>``
- Dividers with ID = ``<div id='enteranamehere'>``
- Dividers with class = ``<div class='enteranamehere'>``
- Text = ``<h> </h>``
- Text Size = <h insertnumberhere> </h insertnumberhere> for text size, smaller = bigger, u can only use 1-6

Links
- Link ``<a href="https://example.com">This is the phrase your link is displayed as</a>``
- Link - Opens in new tab = ``<a href="https://example.com" target="_blank">This is the phrase your link is displayed as</a>``
- Linking to a File = ``<a href="see-below-info_path_to_file" target="_blank">This is the phrase your link is displayed as</a>``
- Image with Link = ``<a href="https://example.com" target="_blank"><img src="INSERT-LINK-TO-IMAGE" alt="This is the phrase your link is displayed as"/></a>``

**Read if linking to a file**\
Use ./filename.filetype if the local file is in the same folder as the website.\
Else use /folder/filename.filetype if its elsewhere.

**Other stuff like images, videos, tables, bold text etc are listed below.**

# Template

#### Before starting, we need to make sure the code is recognised as html

Put ``<!DOCTYPE html>`` on the first line\
Also embed your code between:
````
<html>

</html>
````


- Inside the html tags add a ``<head> </head>`` - this includes website metadata - refer to my metadata section for info (optional)

- inside the head tags, or html tags if you chose not to include a head tag , place ``<body> </body>``  - this tag includes all your html code

#### So now your code should look like this:
````<!DOCTYPE html>
<html>
  <head>
    <body>
      Insert the rest of your html code here now
    </body>
  </head>
</html>
````

# Styling Html

Italics
---

``<em> </em>`` for italic text. put this after ``<h>`` (which is text) to make the ``<h>`` text italic.

E.g\
``<h><em> italic text here </em> normal text here </h>``

Bold Text
---
Similar to above just use ``<strong></strong>``

Line Gaps (Breaks)
---
``<br>`` for a break (gap between lines, as normal enters wont show in html)
this does not need to be ended, just one ``<br>`` per gap wanted.

# Media 

Inserting Images
---

``<img src="link-to-image-here" />``

To insert an image just enter the link to the image after "src=", or the the name of the file if the image is stored locally
You do NOT need to end this tag with </img>, since it has a / at the end inside the <>, it is considered -Self Closing-.

Invisible Image Descriptions 
---

``<img src="link-to-image" alt="image description here" />``

Why is this important? If an image fails to load for a user, it'll at least show a description. For visually impaired people, a screen reader will read this image. And most importantly, many search engines will read the description and show to users when they search the term as search engines cannot see images.

Inserting Videos
---

unlike images, this needs to be closed/ended

````
<video src="link-to-video" width="number-here" height="number-here" controls>
  Video not supported
</video>
````

The text "video not supported", will only be shown if the video fails to load.

# Lists

Unordered Lists - lists are displayed with bullet points
---

ul contains the list items. li is the list item
````
<ul>
  <li> item 1 </li>
  <li> item 2 </li>
</ul>
````

Ordered lists - lists are numbered
---

````
<ol>
  <li> list item one </li>
  <li> list item two </li>
<ol>
````

# Tables 

Table Rows
---

````
<table>
  <tr>
  </tr>
  <tr>
  </tr>
</table>
````
tr is a row, in the above example i've added two.

Tablet Cells
---

just add a ``<td> </td>`` inside your table row above
place any wanted text inside the table cell


# Other 

Linking to Certain Parts of the Same Website
---

Assign an id or div to whatever you want to link to. Example is below:

``<p id="top">This is the top of the page!</p>``

We've assigned an id to that paragraph\

Now we need to call it via a button

````
<ol>
  <li><a href="#top">Top</a></li>
</ol>
````

That list item will link to the #id when clicked. Href can be files, id's or links.

# Metadata 

Tab Name 
---
 
``<title> tab-name-here </title>``

Website Encoding 
---

The website's "encoding" is simply the character set it uses,
most the time this is utf-8, so if you're unsure either leave this or just use the below line

``<meta charset="utf-8">``

(meta tag does not need to be ended)

Search Engine Optimisation
---

Search engines rely on the below metadata, it will use these to display search results.

``<meta name="description" content="website description here">``\
``<meta name="keywords" content="tag1, search-term-tag2, word3">``



