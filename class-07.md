# **Chapter 6:Tables(html)**:

> BASIC TABLE STRUCTURE:

  * The `<table>` element is used to creat a table. The contents of the table are written out row by row. To start earch row you would use a `<tr>` tag (tr stands for table row). Each cell of a table is represented using the `<td>` tag

    * Example:
    
    <table>
      <tr>
        <td>tacos</td>
        <td>Whiskey</td>
        <td>Friends</td>
      </tr>
    </table>

> TABLE HEADINGS:

  * Using the `<th>` element is used like the `<td>` element but its purpose is the represent the table heading for either a column or a row.

> SPANNING COLUMNS:

  * Somtimes you may need the entries in a table to stretch across more then one column. The colspan attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across.

  * Example:

      <table>
        <tr>
          <th></th>
          <th>7am</th>
          <th>8am</th>
          <th>9am</th>
      </tr>
      <tr>
        <th>Feeding time</th>
        <th colspan="2">Charlie</th>
        <td>One scoop</td>
        <td>One cookie</td>
      </tr>
      <tr>
        <th>Feeding time</th>
        <td coolspan="3">Ganon</td>
        <td>One and a half scoop</td>
        <td>One cookie</td>  
      </tr>
    </table>


> SPANNING ROWS:

  * You also may need entries in a tavle to stretch down across more than one row. The rowspan attribute can be used on a `<th>` or `<td>` element to indicate how many rows a cell should span down the table.

    * Example:

      <table>
        <tr>
          <th></th>
          <th>ABC</th>
          <th>BBC</th>
          <th>CNN</th>
        </tr>
        <tr>
          <th>6pm - 7pm</th>
          <td rowspan="2">Movie</td>
          <td>Comedy</td>
          <td>News</td>
        </tr>
        <tr>
          <th>7pm - 8pm</th>
          <td>Sport</td>
          <td>Current Affairs</td>
        </tr>
      </table>

> LONG TABLES:

  * There are three elements that help distinguish between the main content of the table and the first and last rows(which can contain different content). These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table. `<thead>`, `<tbody>`, `<tfoot>`.

    * EXAMPLE:

<table>
  <thead>
    <tr>
      <th>Date</th>
      <th>Income</th>
      <th>Expenditure</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1st January</th>
      <td>250</td>
      <td>36</td>
    </tr>
    <tr>
      <th>2nd January</th>
      <td>285</td>
      <td>48</td>
    </tr>
    <!-- additional rows as above -->
    <tr>
     <th>31st January</th>
     <td>129</td>
     <td>64</td>
    </tr> 
  </tbody>
  <tfoot>
    <tr>
      <td></td>
      <td>7824</td>
      <td>1241</td>
    </tr>
  </tfoot>
</table>

## CHAPTER 3(JAVASCRIPT&JQUERY); FUNTIONS, METHODS, AND OBJECTS:

  > Creating objects using constructor syntax:

  * In the example there is a empty object using the constructor function. Once it has been created, three properties and a method are then assigned to the object. To access a pro 
