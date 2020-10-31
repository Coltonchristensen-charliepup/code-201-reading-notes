# **Chapter 16; IMAGES:**

> Specify the size and alignment of an image using CSS:
 
  * You can specify using img.large, image.medium, and img.small.
  
  * `img.large{`
  * `width:`
  * `height:`
  * `}`

  * To align a image using CSS you would use:

  * `img.aling-left {`
      `float: left;`
      `margin-right: 10px;`
  `}`
  * `img.align-right {`
      `float: right;`
      `margin-left: 10px;`
  `}`
  * `img.medium {` 
    `width: 250px;`
    `height: 250px;`
  `}`

  * Centering a image using CSS you would use:

  * `img.align-center {` 
      `display: block;`
      `margin: 0px auto;`
    `}`
  * `img.medium {`
      `width: 250px;`
      `height: 250px;`
    `}`
> Add background images to boxes:

  * The background-image property allows you to place an image behind any HTML element.

  * `body {` 
      `backgroung-image: url("images/pattern.gif");`
    `}`

  * Repeating images:

  * repeat: will repeat horizontally and vertically.

  * repeat-x: only repeats horizontally.

  * repeat-y: only repeats vertically.

  * no-repeat: image is only shown once.

  * fixed: the background image stays in the same position on the page.

  * scroll: background image moves up and down as the user scrolls.
  
  *  `body {` 
      `background-image: url("images/header.gif");`
      `background-repeat: repeat-x;`
    `}`
> Create image rollovers in CSS:

  * image rollovers & sprites: using CSS, it is possible to create a link or button that changes to a second style when a user moves their mouse over it(known as a rollover)and a third style when they click on it.

    * `<a class="button" id="add-to-basket"> Add to basket</a>`
    
    * `<a class="button" id="framing-options">Framing options</a>`