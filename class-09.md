# CHAPTER 9: (LIST, TABLES AND FORMS)

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