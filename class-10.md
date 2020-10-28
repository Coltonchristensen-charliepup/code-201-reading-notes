# **Chapter 10 Error Handling & Debugging(js)**

> Understanding Errors:

* If a JavaScript statement genereates an error, then it throws an exceprion. At that point, the interpreter stops and looks for exception-handling code.

> Error objects:

* Error objects can help you find where your mistakes are and browsers have tools to help you read them.

  * property description
  
  * name | type of error : syntaxError, ReferenceError, TypeError, RangeError

  * message | description

  * fileNumber | name of the JavaScript file
  
  * lineNumber | line number of error


> How to deal with errors:

* 1: Debug the script to fix errors

* 2: Handle errors gracefully

> A debugging workflow:

* Debugging is about deduction: eliminating potential causes of an error. 

  * Where is the problem? First you should try to narrow down the area where the problem seems to be. In a long script, this is especially important. Second you'll wanty to check how far the script is running. Third use breakpoints where things are going wrong.

  * Browser dev tools also help a tremendously.

> More console methods:

* to differentiate between types of messages you write to the console, you can use three different methods. They use various icons and/or colors to distinguish them.

  * 1: `console.info();` can be used for general information

  * 2: `console.warn();` can be used for warnings

  * 3: `console.error();` can be used to hold errors.

> Group messaging: 

* If you want to write a set of related data to the console, you can use the `console.group()` method to group the messages together.

* When you have finished writing out the results for the group, to indicate the end of the group the `console.groupEnd()` method is used.

