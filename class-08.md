# **Chapter 15 layouts**

> Normal Flow(position:static)

  * In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be: position: static;

    * Example(HTML):

      `<body>`
        `<h1>The Evolution of the bicycle</h1>`
        `<p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster...</p>`
      `</body>`

    * Example(CSS):

      `body {`
        `width: 750px;`
        `font-family: Arial, Verdana, sans-serif;`
        `color: #665544;}`
      `h1 {`
        `background-color: #efefef;`
        `padding: 10px}`
      `p {`
        `width: 450px;}`    

> Relative Positioning(position:relative):

  * Relative positioning moves an element in relation to where it would have been in normal flow.

    * Example:
 
      `p.example {`
        `position: relative;`
        `top: 10px;`
        `left: 100px;`
      `}`

> Absolute Positioning(position:absolute)

  * When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page.

    `h1 {`
      `position; fixed;`
      `top: 0px;`
      `left: 500px;`
      `width: 250px;}`

    `p {`
      `width: 450px;}`


> Fixed positioning(position:fixed):

  * Fixed positioning is a type of absolute positioning tht requires the position property to have a value of fixed. it positions the element in relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exavt same place.

    * Example:
      
      `h1 {`
        `position: fixed;`
        `top: 0px;`
        `left: 0px;`
        `poadding: 10px;`
        `margin: 0px;`
        `width: 100%;`
        `background-color: #efefef;}`
      `p.example {`
        `margin-top: 100px;}`

> Overlapping Elements(z-index):

  * when you use relative, fixed, or avbsolute positioning, boxes can overlap. If boxes overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page.

    * Example: 

       `h1 {`
        `position: fixed;`
        `top: 0px;`
        `left: 0px;`
        `margin: 0px;`
        `poadding: 10px;`
        `width: 100%;`
        `background-color: #efefef;`
        `z-index: 10;}`
      `p.example {`
        `position: relative:`
        `top: 70px;`
        `left: 70px;}`

> Floating Elements(float):

  * The float property allows you to take an element in normal flowand place it as far to the left or right of the containing element as possible.

    * Example(HTML):
      
      `<h1>The Evolution of the bicycle</h1>`
      `<blockquote>"Life is like riding a bicyle. To keep your balance you must keep moving." Albert Einstein</blockquote>`
      `<p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster...</p>`
    
    * Example(CSS):

      `blockquote {`
        `float: right;`
        `width: 275%;`
        `font-size: 130px;`
        `font-style: italic;`
        `font-family: Georgia, times, serif;`
        `margin: 0px 0px 10px 10px;`
        `poadding: 10px;`
        `border-top: 1px solid #665544;`
        `border-bottom: 1px solid #665544;}`


> Using float to place elements side-by-side:

  * A lot of layouts place boxes next to each other. The float property is commonly used to achieve this. When elements are floated, the height of the boxes can affect where the following elements sit.

    * Example(HTML): 
    
    `<body>`
      `<h1>The Evolution of the bicycle</h1>`
      `<blockquote>"Life is like riding a bicyle. To keep your balance you must keep moving." Albert Einstein</blockquote>`
      `<p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster...</p>`
    `</body>`  

  * Example(CSS):

    `body {`
      `width: 750px;`
      `font-family: Arial, Verdana, sans-serif;`
      `color: #665544;}`
    `p {`
    `width: 230px;`
    `float: left;`
    `margin: 5px;`
    `padding: 5px:`
    `backgound-color: #efefef;}`

> Clearing Floats(clear):

  * The clear property allows you to say that no element(within the same containing element) sould touch the left or right-hand sides of a box. It can take the following values:

    * Left: The left-hand side of the box should not touch any other elements appearing in the same containing element.

    * Right: The right-hand side of the box should not touch any other elements appearing in the same containing element.

    * Both: Neither left nor right-hand side of the box will touch elements appearing in the same containing element.

    * None: Elements can touch either side. 

  * Example(HTML): 
  
    <p class="clear">In 1865, the Velocipede attached pedals to the front wheel, but its wooden structure made it extremely uncomfortable.</p>

  * Example(CSS):

    `body {`
      `width: 750px;`
      `font-family: Arial, Verdana, sans-serif;`
      `color: #665544;}`
    `p {`
      `width: 230px;`
      `float: left;`
      `margin: 5px;`
      `padding: 5px;`
      `background-color: efefef;}`
    `.clear {`
      `clear: left;}`    
      