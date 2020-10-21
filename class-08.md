# **Chapter 15 layouts**

> Normal Flow(position:static)

  * In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be: position: static;

    * Example(HTML):

      <body>
        <h1>The Evolution of the bicycle</h1>
        <p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster...</p>
      </body>

    * Example(CSS):

      body {
        width: 750px;
        font-family: Arial, Verdana, sans-serif;
        color: #665544;}
      h1 {
        background-color: #efefef;
        padding: 10px}
      p {
        width: 450px;}    

> Relative Positioning(position:relative):

  * Relative positioning moves an element in relation to where it would have been in normal flow.

    * Example:
      p.example {
        position: relative;
        top: 10px;
        left: 100px;
      }


> Absolute Positioning(position:absolute)

  * When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page.

    h1 {
      position; fixed;
      top: 0px;
      
    }