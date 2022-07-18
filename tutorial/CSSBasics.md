
CSS provides the vocabulary to tell a web browser things like,
“I want my headings to be really big and my sidebar to appear on the left of the main article.” 
HTML doesn’t have the terminology to make those kinds of layout decisions—all it can say is, 
“that’s a heading and that’s a sidebar.”

Note that there’s no direct connection between the browser and our stylesheet. 
It’s only through the HTML markup that the browser can find it. CSS, images, and even JavaScript 
all rely on an HTML page to glue everything together, making HTML the heart of most websites.

It’s almost always better to store all your CSS in external stylesheets opposed to style elements in each html file.
Inline styles should be avoided at all costs because they make it impossible to alter styles from an external stylesheet.



*CSS Structure*

"Selector"  "Property"    "Value"
body          {color   :  #FF0000  }

Linking a CSS Stylesheet
<link/> only used in  <head> </head>
<link rel='stylesheet' href='css file reference'/>

Units of Measurement
px (pixel)
em (defines sizes relative to some base font)

Select multiple HTML in the same CSS with commas
h1, h2, h3, h4 {
...
}

List Styles 
define <ul> (unordered list) or <ol> (ordered list)
list-style-type: circle; (non filled circle)
list-style-type: lower-roman; (roman numbers)

Block Elements and Inline Elements
display: block;
display: inline; 

*CSS Box-Model*

"Content  Padding  Border and Margin"

Content 
*The text, image, or other media content in the element.*

Padding 
*The space between the box’s content and its border.*

Padding: Vertical Horizontal
Padding: Top Right Bottom Left

p {
  padding: 20px(vertical) 10px (horizontal);  /* Vertical  Horizontal */
}

or

p {
  padding-top: 20px;
  padding-bottom: 20px;
  padding-left: 10px;
  padding-right: 10px;
}

or 

p {
  padding: 20px (top) 0(right) 20px(bottom) 10px(left);  /* Top  Right  Bottom  Left */
}

Border 
*The line between the box’s padding and margin.*


Borders 

Borders:       Size Style Color
border-bottom: 1px  solid #5D6063;

Margins
*The space between the box and surrounding boxes.*
example

p {
  padding: 20px 0 20px 10px;
  margin-bottom: 50px;          /* Add this */
}

Preventing Margin Collapse 
1. Adding an element with non zero height for consecutive elemnts to collapse into
2. Only using Padding for spacing instead of margin (cant use padding for anything else)
3. top or bottom-only convention - If only one vertical margin is defined the elements cant collapse


Generic Boxes
<div> and <span> are “container” elements that don’t have any affect on the semantic structure of an HTML document.^
hey do, however, provide a hook for adding CSS styles to arbitrary sections of a web page.

Centering with Auto-Margins
Set block level to "auto" -> margin: 20px auto; (Only works with explicit width)

Resetting Styles 
* (on top of the page)= Resets the padding and margin properties

Basic Link Styles

:link – A link the user has never visited.
:visited – A link the user has visited before.
:hover – A link with the user’s mouse over it.
:active – A link that’s being pressed down by a mouse (or finger).

example: 
a: link {
   color: purple;
}

Creating Buttons that switch color when hovering and clicking

example:
  .button:active, 
  .button:visited:active{
    color: #FFF;
    background-color:#5995DA;
  }

.call-to-action:link,
.call-to-action:visited{
  font-style: italic;
  background-color: #EEB75A;
}

.call-to-action:hover,
.call-to-action:visited:hover{
  background-color:#91e09f;
}

.call-to-action:active,
.call-to-action:visited:active{
  background-color: #2a23e0;
}

Different ways of working 
Pseudo Classes - :first-of-type / :last-of-type
ID Selectors   - id attribution on HTML elements








