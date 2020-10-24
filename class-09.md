# CHAPTER 7: (FORMS)

> form structure:

  * Form controls live inside a `<form>` element. This element should always carry the action attribute and will usually have a method and id attrubute too. Action of a form: every `<form>` element requires an action attribute. It's value is the URL for the page on the server that will receive the information in the form when it is submitted. Methods in a form: forms can be sent using one of the two methods: get or post.

    * `<form action="http://www.example.com/subscribe.php" method="get">`
          `<p> this is where the form controls will appear.</p>`
      `</form>`   

> text input:

  * The `<input>` element is used to create several different form controls. The value of the type attribute determines what kind of input they will be  creating

    * type="text" when the type attribute has a value of text, it creates a single-line text input. 

## CHAPTER 14: (LIST, TABLES AND FORMS)

> bullet point styles:

  * css you would use list-style-type

  example: ol {
  list-style-type: lower-roman;}

  * html you can use a <ul></ul> tag with <li></li> tags in between to get your unordered list

> images for bullets:

  * css you would use list-style-image

    * example:
    ul {
      list-style-image: url("images/star.png");}
    li {
      margin: 10px 0px 0px 0px;}
    
> positioning the marker

  * css list-style-position

> list short hand

 * css list-style

> table properties

  * html: 

  <h1>First edition auctions</h1>
   <table>
    <tr>
      <th>Aurtor</th>
      <th>Title</th>
      <th class="money">reserve price</th>
      <th class="money">current bid</th>
    </tr>
  </table>

  * css

  body {}
  
  table {}

  th, td {}

  th {}

  tr.even {}

  .money {}


> border on empty cells

  * css empty-cells

    * you would find this wrapped in table.one or table.two{empty-cells: show}


> gaps between cells

  * css borer-spacing, border-collapse