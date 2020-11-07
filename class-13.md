# **Local Strorage**

> HTML Storage Support

* IE`(8.0+)`

* FIREFOX`(3.5+)`

* SAFARI`(4.0+)`

* CHROME`(4.0+)`

* OPERA`(10.5+)`

* IPHONE`(2.0+)`

* ANDROID`(2.0+)`

> Check For HTML5 storage:

* Example: 

  * `function supports_html5_storage() {`
  `try {`
    `return 'localStorage' in window &&` `window['localStorage'] !== null;`
  `} catch (e) {`
    `return false;`
  `}`
`}`

* HTML5 storage is based on named key/value pairs. you store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parsFloat()` to coerce your retrieved data into the expected JavaScript datatype.

  * Example:

    * `interface Storage {`
  `getter any getItem(in DOMString key);`
  `setter creator void setItem(in` `DOMString key, in any data);`
`};`


* Calling `setItem()` with a named key that already exists will silently overwrite the previous value. Calling 
`getItem()` with a non-existent key will return null rather than throw an exception.

* Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the `getItem()` and `setItem()` methods, you can simply use square brackets. 

* Example:

  * `var foo = localStorage.getItem("bar");`
    `// ...`
    `localStorage.setItem("bar", foo);`
    
    * …could be rewritten to use square bracket syntax instead:

* `var foo = localStorage["bar"];`
  `// ...`
  `localStorage["bar"] = foo;`

* There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

* `interface Storage {`
  `deleter void removeItem(in DOMString key);`
  `void clear();`
`};`

* Calling `removeItem()` with a non-existent key will do nothing.

* Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

* Example:

  * `interface Storage {`
    `readonly attribute unsigned long length;`
    `getter DOMString key(in unsigned long index);`
  `};`


* If you call `key()` with an index that is not between 0–(length-1), the function will return null.