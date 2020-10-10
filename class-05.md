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



# **Chapter 12**:

  > *TEXT*:

  * Specifying typefaces(font-family): The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

    * Example: `<!DOCTYPE html>`
                  `<html>`
                    `<head`>
                      `<title>font family</title>`
                      `<style type="text/css">`
                        `body {`
                          `font-family: Gorgia, Times, serif;}`
                        `h1, h2 {`
                          `font-family: Arial, Verdana, sans-serif;}`
                        `.credits {`
                          `font-family: "Courier New", Courier, monospace;}`
                      `</style>`
                    `</head>`
                    `<body>`
                      `<h1>Briards</h1>`
                      `<p class="credits">by Ivy Duckett</p>`
                      `<p class="inro">The <a class="breed" href="http://en.wikipedia.org/wiki/Briard">briard</a>, or berger de brie, is a large breed of dog traditionally used as a herder and guardian of sheep...</p>`
                    `</body>`
                  `</html>`

  
  * SIZE OF TYPE(font-size): This enables you to specify a size for the font. There are several ways to specify the size of a font.

    * Examples:

      * PIXLES: commonly used because they allow web designers very precise control over how much space their text taxes up. The number of pixles is followed by the letters px.

      * PERCENTAGES: The default size of text in browsers is 16px. So a size of 75% would be equivalent of 12px, and 200% would be 32px.

      * EMS: An em is equivalent to the width of a letter m.

      * More font choices(@font-face): Which this allows you to use fonts even if they aren't installed on the computer of the person browsing.

      * Understanding font formats: Different browsers support different formats for fonts(in the same way that they support different audio and video formats, so you will need to supply the font in several variations to reach all browsers.

      * BOLD(font-weight): The font-weight property allows you to create bold text. There are two values that this property commonly takes: 

        * normal: this causes text to appear at a normal weight.

        * bold: This causes text to appear bold.

      * ITALIC(font-style): If you want to create italic text, you can use the font-style property. There are three values this property can take: 

        * Normal: This causes text to appear in a normal style(as opposed to italic or oblique).

        * Italic: This causes text to appear italic.

        * Oblique: This causes text to appear oblique.

      * UPPERCASE & LOWERCASE(text-transform):

          * text-transform: uppercase; will uppercase your text

          * text-transform: lowercase; will lowercase your text

          * text-transform: capitalize; will cause the first letter of each word to appear capitalized.

      * UNDERLINE & STRIKE(text-decoration):

        * text-decoration: none; removes an decoration that has already been applied

        * text-decoration: underline; add a underline

        * text-decoration: overline; adds a line over the top

        * text-decoration: line-through; adds a line through words

        * text-decoration: blink; this animates the text to make it flash on and off(however this is generally frowned uppon, as its considered annoying).

      * LEADING(line-height): p{ line-height: 1.4em;} This is generally used as a term for the vertical space between lines of text.

      * LETTER & WORD SPACING(letter-spacing, word-spacing): Typographers use for the space between each letter. h1, h2{text-transform: uppercase; letter-spacing: 0.2em;}
      .credits {
        font-weight: bold;
        word-spacing: 1em;}

        * text-align:(left, right, center, justify)

        * vertical-algin:(baseline, sub, super, top, text-stop, middle, bottom, text-bottom).

        * text-indent: 20px; That is a example of which it allows you to properly indent your text.

        * text-shadow: 
        p.one{
          background-color: #eeeeee;
          text-shadow: 1 1 0 #000000;}
          
          * This is used to create a drop shadow, which is a dark version of the word just behind it and slightly offset.

          