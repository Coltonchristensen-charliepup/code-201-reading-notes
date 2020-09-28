INTRODUCTION:
Goes over how HTML & CSS work. Along with helping you understand that you don't have to be a genius to read, write, and explain how it all works.
For instense Html is the structure of the page, <Head>, <titles>, <body>, <h1> and so forth are all examples of things on a web page. So what do some of these things do?
Well for instense the <head> indicates the begining of your page <title> follows underneath it to give you the file name and or page name although you wont be able to see these things on a web page they typically reside in the url. The header is the first thing on a webpage it is what greates you unless you have a <script> on your page then that is what you will see first!
  
  Quiz question: What is the <body> tags funtion?
  a. to talk about the human body!  
  b. the structure of your page that holds all your content!
  c. helps define a dogs body.
  d. none of the above.
  
 STRUCTURE:
 This chapter goes over about, tags and elements. Headings and Subheadings in any document often show the importance of the content. 
Which is expanded by subheadings lower on the page, usually followed by a paragraph that explains each topic. code example that will help you understand your webpage format.
<html>
  <body>
    <h1>This is the Main Heading</h1>
    <p>This text might be an introduction to the rest of the page. And if the page is a long one it might be split up into sereal sub-headings.</p>
    <h2>This is a sub-heading.</h2>
    <p>Many long articles have sub-headings to help you follow the structure of what is being written. There may even be sub-sub-headings (or lower-level headings).</p>
    <h2>Another sub-heading</h2>
    <p>Here you can see another sub-heading</p>
  </body>
</html>

The html code inside the angled brackets are called elements. Elements are typically made up of two tags a opening and a closing tag (<this opens></this closes>). Although what i have put inside my open and closing tags are not actual elements i put them there as a reference for users to remember the order of there opening and closing tags.

Quiz question: When you open and close a tag where does the information go?
a: before the tags
b: after the tags
c: in between the tags
D: none of the above.

Attributes provide aiddtional information about the contents of a element. They are located in the opening tag of the element and are made up of two parts: name and a value seperated by a equals sign(=). <p lang="en-us">Paragraph in English</p> if you change it to <p lang="fr">Paragraph en Francais</p>. majority of attribues can only appear in certain elements, although a couple can appear on any element such as (lang).

CHAPTER 8 Extra Markup:
There are different types of html:
*Html 4 released in 1997
*Xhtml 1.0 released in 2000
*Html 5 work in progress

Ever since the web was created there have been several different verions of html. Each different version was designed to be an improvement. Seeing how there are many different types of you should always start your web page with a DOCTYPE declaration to tell the browser which version of HTML the page is using. 
HTML5: <!DOCTYPE html>
HTML 4: <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
 TRANSITIONAL XHTML 1.0: <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
STRICT XHTML 1.0: <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
XML DECLARTION: <?xml version="1.0" ?>

ID ATTRIBUTE:
Every HTML element can carry the id element which is used to uniquely identify that element from other elements on the page.
These should start with a letter or a underscore(not a number or any other character). Make sure that you don't have multiple elements on the page with the same value for their id attributes, if you do the value is no longer unique. <p id="name"> this will show you the name you have rendered in bold text. 
CLASS ATTRIBUTE: <p Class="n ">



