# Chapter 5 Html&Css 

> Images 

* Adding Images: To add a image into the page you will need the `<img>` element. Which is a empty element so there is no closing tag.

  * Example: `<img src="images/quokka.jpg" alt="A family of quokka" title="The Quokka is an Australian marsupial that is similar in size to the domestic cat." />`

* Height and Width of images: You will often see the `<img>` element us two other attributes that specify its size. Which is [height and width].

  * Example: `<img src="images/quokka.jpg" alt="A family of quokka" width="600" height="450" />`

* Where to place images in your code: Depending on where you place the image in your code will determine how it is displayed.

  * One: **BEFORE A PARAGRAPH**; The paragraph starts on a new line after the image 
  
  * Two: **INSIDE THE START OF A PARAGRAPH**; The first row of text aligns with the bottom of the image.

  * Three: **IN THE MIDDLE OF A PARAGRAPH**; The image is placed between the words of the paragraph that it appears in.

* OLD CODE: ALIGNING IMAGES HORIZONTILLY:

  * **ALIGN**: The align attribute was commonly used to indicate how the other parts of a page should flow around a image. But unfortunately the align attribute is no longer used in html5. Here are some examples of what it used to look like (`align="left"`); This will align the image to the left(allowing text to flow around the right hand side). Or you can `align="right"` and this will align the image to the right(allowing the text to flow around the left hand side).

> HTML5: FIGURE AND FIGURE CAPTION:

  * Images often come with captions. With the update of HTML5 it introduced the `<figure>` element. Along with the `<figcaption>` element.

    * Examples:

        `<figure>`
          `<img src="images/otters.jpg" alt="Photograph of two sea otters floating in water" />`
        `<br />`
          `<figcaption>Sea otters hold hands when they sleep so they don't drift away from each other.</figcaption>`
        `</figure>` 


# **Chapter 11 Hmtl:**

  > COLORS:

  * **Foreground color**: The color property allows you to specify the color of text inside an element.

    * RGB values, express colors in terms of how much red, green, and blue are used to make it up. example: rgb(100,100,90).

    * Hex Codes, are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. Example: (#ee3e80).

    * Color Names, There are 147 predefined color names tat are recognized by browsers. Example: (DarkCyan).

  * **Background color**: CSS treats each HTML element as if it appears in a box, and the `background-color` property sets the color of the background for that box.  

  * **Contrast**

    * CSS3: Opacity(`opacity, rgba`); this allows you to specify the opacity of a element and of any of it's child elements. The value is a number between 0.0 and 1.0(so a value of .5 is 50% opacity and .15 is 15% opacity) `p.one{background-color: rgb(0,0,0); opacity: 0.5;} 0.two{background-color: rgb(0,0,0); background-color: rgba(0,0,0,0.5);}`

    * CSS3: HSL & HSLA(`hsl, hsla`); The hsl color property has been introduced n CSS3 as an altenative way to specify colors. The value of the property starts by individual values inside parentheses for: 

      * HUE: This is expressed as an angle(between 0 and 360 degrees).
      
      * SATURATION: This is expresed as a percentage.

      * LIGHTNESS: This is expressed as a precentage with 0% being white, 50% being normal, and 100% being black.
      
      * ALPHA: This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.



  