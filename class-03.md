# Html Chapter 3: lists

> **Numbered list:**
  - ordered lists
  `<ol></ol>` are created with these elements and inside them the `<li></li>` tag reside.
  - example: 
  <ol>
  <li>milk</li>
  <li>eggs</li>
  <li>bacon</li>
  </ol>

> **Bullet lists:**
  - unordered lists
    `<ul></ul><li></li>`
    - The unordered list is created with the `<ul></ul>` element
    - Each item is place between an opinging `<li> ` tag and a closing `</li>` tag
    - example:
  
  `<ul>`
      <li>charlie</li>
      <li>ball</li>
      <li>endless field</li>
  `</ul>`
  

> **Definition lists:**
  
  - This list is started with the `<dl>` element and closed with the `</dl>` element. Inside the `<dl>` element you will typically see pairs of `<dt>` and `<dd>` elments. `<dt>` This is used to contain the term being defined(the definition term). `<dd>` This is used to contain the definition. You may see a list where two terms were used for the same definition.


> **Nested lists:**

  - These are used to put a second list inside of a `<li>` element to create a sub-list or nested list. 
  - Example: 
  <ul>
    <li>Coffee</li>
    <li>Muffin
     <ul>
      <li>Dog</li>
      <li>Park</li>
      <li>Chuck-it</li>
      <li>Ball</li> 
     </ul>
    </li>
   <li>The morning routine</li>
  </ul>


## (JS) Chapter 2 pg(70-73):

  > Arrays
  * Are created just like any other variable by using the var keyword followed by the name of the array. The values are assigned to the array using square brackets `[]`, and each value is seperated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a boolean all in the same array. The technique for creating an array is known as an array literal. It is usually the prefferred method for creating an array. You can alsowrite each value on a separate line.
  colors = ['white','black','custom'];

  * Examples:
    * var colors;
    * colors = ['white', 'black', 'custom']
    * var el = document.gitElementById('colors');
    * el.textContent = colors[0];

    * var colors = new Array('white', 'black', 'custom');
    * var el = document.getElementsById('colors');
    * el.textContent = colors[0];

> Values in arrays

  * Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of the list starts at zero (not one).

    - Numbering items in an array:

    `var colors;`

    `colors = ['white',` 
    
    `        'black',`
    
    `        'custom'];`

    - Accessing items in an array:

    `var itemThree;`

    `itemThree = colors[2];`

    - Number of items in an array




  

