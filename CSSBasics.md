
CSS provides the vocabulary to tell a web browser things like,
“I want my headings to be really big and my sidebar to appear on the left of the main article.” 
HTML doesn’t have the terminology to make those kinds of layout decisions—all it can say is, 
“that’s a heading and that’s a sidebar.”

Note that there’s no direct connection between the browser and our stylesheet. 
It’s only through the HTML markup that the browser can find it. CSS, images, and even JavaScript 
all rely on an HTML page to glue everything together, making HTML the heart of most websites.

It’s almost always better to store all your CSS in external stylesheets opposed to style elements in each html file.
Inline styles should be avoided at all costs because they make it impossible to alter styles from an external stylesheet.



CSS Structure
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







