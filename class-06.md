# **Chapter 3 js book:**

  > Objects:
   * creating objects using literal notataion: The example starts by creating an object using literal notion. the object is called *hotel* whic represents a hotel calld *Quay* with 40 rooms (25 which have been booked). Next the content of the page is updated with data from tis object. It shows th name of the hotel by accessing the objects name property and the number of vacant rooms using the checkAvailability() method. 

      * var hotel = {
        name: 'Quay',
        rooms: 40,
        booked: 25,
        checkAvailability: function() {
          return this.rooms - this.booked;
        }
      };

      var elName = document.getElementById('hotelName');
      elName.textContent = hotel.name;

      car elRooms = document.getElementById('rooms');
      elRooms.textConten = hotel.checkAvaliability();


  * Creating more object literals:

    * var hotel = {
      name: 'Park',
      rooms: 120,
      booked: 77,
      checkAvaliability: fuction(){
        return this.rooms - this.booked;
      } 
    };    

    var elName = document.getElementById('hotelName');
    elName.textContent = hotel.name;

    var elRooms = document.getElementById('rooms');
    elRooms.textContent = hotel.checkAvailability();


## **Chapter 5 Document, Object, Model:**

  * The document object model(DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
  
  > Working wiht the DOM tree:

    * Accessing and updating the DOM tree involes two steps:
      
      * 1: Locate the node that represents the element you want to work with.
      
      * 2: Use its text content, child elements, and attributes.

    > Accessing Elements:

      * DOM queries may return one element, or they may return a Nodelist, which is a collecion of nodes.
        * Methods that return a single element node:

        * getElementById('id'): selects an individual element given the value of its id attribute. The HTML must have a n id attribute in order for it to be selectable.

        * querySelector('css selector'): Uses CSS selector syntax that would select one or more elements. This method returns only the first of the matching elements.

        * Methods that return one or more elements(as a Nodelist):

          * getElementsByClassName('class'): selects one or more elements given the value of their class attribute.

          * getElementsByTagName('tagName'): selects all elements on the page with the specified tag name. This method is faster than querySelectorAll().

          * querySelectorAll('css selector'): Uses CSS selector syntax to select one or more elements and returns all of those that match.

    > Selecting Elements Using ID Attributes:

      * getElementById(), allows you to select a single element node by specifying the value of its id attribute

        * Example HTML:<h1 id="header">List King</h1>
                  <h2>Buy groceries</h2>
                  <ul>
                    <li id="one" class="hot"><em>fresh</em>figs</li>
                    <id="two" class="hot">pine nuts</li>
                    <li id="three" class="hot">honey</li>
                    <li id="four">balsamic vinegar</li>
                  </ul>

          * JavaScript: // select the element and store it in a variable.
          Var el = document.getElementById('one');

          // cange the value of the class attribute.
          el.className = 'cool';

    > NODELISTS: DOM QUERIES THAT RETURN MOR THAN ONE ELEMENT:

      * getElementsByTagName('h1'): even though this query only returns on element, the method still returns a NodeList because of the potential for returning more than one element.

      * getElementsByTagName('li'): this method returns four elements, one for each of the `<li>` elements on the page.

      * getElementsByClassName('hot'): this NodeList contains only three of the `<li>` elements becasue we are searching for elements by the value of their class attribute, not tag name.

      * querySelectorAll(li[id]): thsi method returns four elements, one for each of the `<li>` elements on the page that have an id attribute(regardless of the values of the id attributes.)