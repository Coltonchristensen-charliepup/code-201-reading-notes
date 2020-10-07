# **Chapter 4(html/css): Links**

> **Writing Links:**

- links are created using `<a>` element. Users can click on anything between the opening `<a>` and closing `</a>` tag. To specifiy which link you want to link to by using the href attribute.

- Linking to other sites:

  - Example
  - `<p>` Movie Reviews:
    `<ul>`
    ` <li>``<a href="http://www.empiroenline.com"> `Empire`</a></li>` `</p>`

- Linking to other pages on the same site

  - Example:
  - `<p>`
    `<ul>`
    `<li><a href="index.html">Home</a></li>`
    `<li><a href="about-us.html">About</a></li>`
    `<li><a href="movies.html">Movies</a></li>`
    `<li><a href="contacts.html"> Contacts</a></li>`
    `</ul>`
    `</p>`

> Email links:

`<a href="mailto:jon@example.org"> Email Jon</a>`

> Opening links in a new window:

- `<a href="http://www.imdb.com" target="blank"> Internet Movie Database</a> (opens in new window)`

> Linking to a specific part of the same page:

- <h1 id="top">Film-terms</h1>
  <a href="#arc_shot">Arc Shot</a><br />
  <a href="#interlude">Interlude</a><br />
  <a href="#prologue">Proglogue</a><br /><br />
  <h2 id="arc_shot">Arc Shot</h2>
  <p>A shot in which the subject is photographed by an encircling or moving camera</p>
  <h2 id="intrerlude">Interlude</h2>
  <p>A brief, intervening film scene or sequence, not specifically tied to the plot, that appears within a film</p>
  <h2 id="prologue">Prologue</h2>
  <p>A speech, preface, introducuton, or brief scene contrast to epilogue</p>
  <p><a href="#top">Top</a></p>

- Linking to a specfic part of another page uses a simular tchnique. As long as the page you are linking to has id attributes that identify specific parts of the page, you can simply add the same syntax to the end of the link for that page.

# Chapter 15(html/css): Layouts

> Normal flow(position:static)

- Html: <body>
    <h1> The evolution ofthe bicycle</h1>
    <p>In 1817 Baron Von Drais invented a walking maching that would help him get around the royal gardens faster...</p>
  </body>

  - Css: Body {
    `width: 750px;`
    `font-family: Arial, Verdana< sans-serif;`
    `color: #6655544}`
    `h1 {`
    `background-color: #efefef;`
    `padding: 10px;}`
    `p {`
    `width: 450px;}`

    > Relative positioning(position:relative)

    - This moves elements in a relation to where it would have been in normal flow

    - Html: is the same as above

    - css:
      p.example {
      position relative;
      top: 10px
      left: 100px
      }

    > Absolute postioning(position:absolute)

    - When the position propery is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements onthe page.

    - Html:

    `<body>`
    `<h1>The evolution ofthe bicycle</h1>`
    `<p>In 1817 Baron Von Drais invented a walking maching that would help him get around the royal gardens faster...</p>`
    `</body>`

    - Css:
      h1 {
      position: absolute;
      top: 0px;
      left: 500px;
      width: 250px;}

      p {
      width: 450px;}

    > Fixed positioning(postition:fixed)

    * `<body>`
        `<h1>The evolution ofthe bicycle</h1>`
        `<p class="example">In 1817 Baron Von Drais invented a walking maching that would help him get around the royal gardens faster...</p>`
    `</body>`

        * Css:

         h1 {
         position: fixed;
         top: 0px;
         left: 0px;
         padding: 10px;
         margin: 0px;
         width: 100px;
         background-color: #efefef;}
         p.example {
           margin-top: 100px}

    > Overlapping Elements(z-index)

    - - Css:

      h1 {
      position: fixed;
      top: 0px;
      left: 0px;
      padding: 10px;
      margin: 0px;
      width: 100px;
      background-color: #efefef;
      z-index: 10px;}
      p.example {
      top: 10px;
      left: 70px;}

  > Floating elements(float)

  * html 
  `<body>`
      `<h1>The evolution ofthe bicycle</h1>`
      `<blockquote>"Life is like riding a bicycle. To keep your balance you must keep moving." Albert Einstein</blockquotes>`
      `<p class="example">In 1817 Baron Von Drais invented a walking maching that would help him get around the royal gardens faster: two same-size in-line wheels, the front one steerable, mounted in a frame...</p>`
    `</body>`
  * css
  blockquote {
    float: right;
    width: 275px;
    front-size: italic;
    font-family: Georgia, Times, Serif;
    margin: 0px 0px 10px 10px;
    padding: 10px
    border-top: 1px solid #665544;
    border-bottom: 1px solid #665544;}


# **Chapter 3 Functions, Methods, and Objects**

  > A Basic Function
  * Html 
  `<!Doctype html>`
  `<html>`
    `<head>`
      `<title>Basic Funtion</title>`
      `<link rel="stylesheet" href="css/c03.css" />`
    `</head>`
    `<body>`
      `<h1>Travel Worthy</h1>`
      `<div id="meassage">Welcome to our site!</div>`
      `<script src="js/basic-funtion.js"></script>`
    `</body>`    
  `</html>`  

  * JavaScript
  `car msg = 'Sign up to receive our newsletter for 10% off!';`
  `function updateMessage() {`
    `var el = document.getElementById('message');`
    `el.textContent = msg;`
  `}`
  `updateMessage();`

  