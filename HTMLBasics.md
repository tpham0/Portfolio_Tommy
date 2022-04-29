Basic Structure
<html>

  <head>
    <!-- Metadata goes here -->
  </head>

  <body>
    <!-- Content goes here -->
  </body>

</html>


Commentary
<!-- -->

Paragraphs
The <p> element marks all the text inside it as a distinct paragraph.

Headings
<h1>, <h2>, <h3>, … , <h6></h6>
"Higher number = less prominant(smaller)"

Unordered Lists (with Dots) Structure 
<ul>
    <li>Random Text</li>
    <li>Add each item in its own "li" element</li>
    <li>They don't need to be in any particular order</li>
  </ul>

Ordered List (numeric) Structure
<ol>
    <li>Notice the new "ol" element wrapping everything</li>
    <li>But, the list item elements are the same</li>
    <li>Also note how the numbers increment on their own</li>
    <li>You should be noticing things is this precise order, because this is
        an ordered list</li>
  </ol>

Text Emphasis
cursiv =           <p><em>...</em></p>
bold   =           <p><strong>...</strong></p>
cursiv + bold =    <p><em><strong>...</strong></em></p>

Empty html elements 
text break = <br/>

Horizontal Rules
Transition from one scene to another = <hr/>
Important to seperate content of Html from Css(presenation)

Trailing Slash to close an element 
<br> vs <br/>
It is optional but useful vor visual reference.

Links are created with anchors 
<a> </a>

- Types of Links -

"Absolute" Use case for directing towards different websites
Structure: Scheme   + Domain                  + Path
           https://   Developer.Mozilla.org   /EN-US/DOCS/WEB/HTML

"Relative" Use case for pointing towards another file on the website
<a href='misc/extras.html'>extras page</a>

Parent Folders



