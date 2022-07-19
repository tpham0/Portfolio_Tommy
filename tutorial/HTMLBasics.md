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

Selectors 
ID selectors:     <a id= 'name class= 'name'> href='link' </a> 
Class selectors:  <div class= 'name'> </div>

CSS Specificity Ranking (High to Low)

#button-2
.button:link
a:link and .synopsis em (they’re equal)
.button
a

Flexbox 

.menu-container {
  display: flex;

Enables the flexbox layout mode, makes it possible to mix and match flexbox with other layout models

 justify-content: 
 center  
 flex-start
 flex-end
 space-around
 space-between

 Flex Container Direction

 flex-direction: column/ row 
 // Can change the direction of the flexboxes 

Flex Direction: Row; 
Vertical = Justify content: 
Horizontal = Align Items

Flex Direction: Column; 
Vertical =  Align Items:
Horizontal = Justify content:

Flex Container Order
flex-direction: row
                row-reverse
                column
                column-reverse

Flex Item Order

.first-item {
  order: 1;
}

.last-item {
  order: -1;
}
// Switches First and Last Item 

Flexible Items

flex: initial (fixed)
      flex 1; (flexible)
      flex 2; (grow twice the size compared to other flex)

Asvanced Positioning 
Relative:  
Absolute:
Fixed:

.item-example{
  postion: relative
           absolute
           fixed:
}

"Navigation menu's should be marked as <ul> instead of <div>" - more accesible for search engines

Responsive Design

@media only screen and (min-width:...px) and (max-width:...px)
  -defining the size of the device

(IN CSS! Important to include this so the website is flexbile) - flex-wrap prpoerty
.page {
  display: flex;
  flex-wrap: wrap;
}

!IMPORTANT! - include within HTML <head>  - disables devices form using default mobile layout which only zooms out of the desktop version.

<meta name='viewport'
      content='width=device-width, initial-scale=1.0, maximum-scale=1.0' />

CSS example:
/* Mobile Styles */
@media only screen and (max-width: 400px) {
  body {
    background-color: #F09A9D; /* Red */
  }
}

/* Tablet Styles */
@media only screen and (min-width: 401px) and (max-width: 960px) {
  body {
    background-color: #F5CF8E; /* Yellow */
  }
}

/* Desktop Styles */
@media only screen and (min-width: 961px) {
  body {
    background-color: #B2D6FF; /* Blue */
  }

  HMTL Semantic
  
  makro:
  Header
  Article <Figure>
  Footer

  Article - independent element
  Section - explicit way to define sections in the document

  Without this <header>, search engines and screen readers wouldn’t know that first <p> was separate from the main content of the article.

Web Forms

<input type='text'/>
<input type='email'/>
<input type='radio'/>
<select> and <option>
<textarea>
<input type='checkbox'/>
<button>


Web Typography

Locally Hosted
1. Install Font
2. Include into Website Folder
3. Include it in Html & CSS

example: include at the very top of CSS
@font-face {
  font-family: 'Roboto';
  src: url('Roboto-Light-webfont.woff') format('woff');
  font-style: normal;
  font-weight: 300;
}

Externally Hosted Web Fonts
1. Choose Google Font
2. Find the Link to Font
3. Embed it into HTML head as a <link>
<link href="https://fonts.googleapis.com/css?family=UnifrakturMaguntia" rel="stylesheet">
4. Add <style> in <head> to include it
<style>
  .blackletter {
    font-family: 'UnifrakturMaguntia', cursive;
  }
</style>


Tips & Tricks
Use a font-size between 14px and 20px for the body element.
Use “curly quotes” and apostrophes with the &rsquo;, &lsquo;, &rdquo;, and &ldquo; HTML entities.
Use proper dashes (&ndash;, &mdash;) and other symbols (&copy;).
Don’t use text-decoration: underline except for hover states.
Use real italic fonts over synthesized ones if not it’s too much of a performance burden.
