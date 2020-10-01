# Chapter 2: text

* **When creating a web page, you add tags(known as markup) to the contents of the page**.

  - Structual markup: the elements that you can use to describe both headings and paragraphs
  - Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quatation(who said it), the meaning of acronyms,and so on.

> HEADINGS
  - html has six "levels" of headings

  - `<h1>this is the main heading</h1>`
  - `<h2>this is a level 2 heading</h2>`
  - `<h3>this is a level 3 heading</h3>`
  - `<h4>this is a level 4 heading</h4>`
  - `<h5>this is a level 5 heading</h5>`
  - `<h6>this is a level 6 heading</h6>`

> PARAGRAPHS
  - to create a paragraph, surround the words that make up the paragraph with a opening(<p>) tag and a closing (</p>) tag.

> BOLD&ITALIC
  - by enclosing words in `<b>` &`</b>` tags we can make them bold.
  - by enclosing words in `<i>` &`</i>` tags we can make words appear italic.

> SUPERSCRIPT&SUBSCRIPT
  - the `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power.
  - the `<sub>` element is used to contain characters that should subscript. It's commonly used with foot notes or chemical formulas
  
> WHITE SPACE
  - This is typically used to make code easier to read. When a browser sees two or more spaces next to each other, it commonly deispalys one space. If it comes across a line break, it will treat it as a single space as well. Which is called a **White space collapsing**.

> LINES BREAKES & HORIZONTAL RULES:
  - `<p>The Earth<br />gets one hundred tons heavier every day<br /> due to falling space dust.</p> ` As you can see, the browser will automatically show you all new paragraphs or headings. If you wanted to add a line break inside the middle of a paragraph you can us the tag shown above

  - `<hr/>` Is used to create a break between themes. There a only a few elements that do not have words between a opening and closing tag. These are called empty elements. Which typically only have one tag. Before the closing angled bracket of an empty element there will often be a space and a forward slash.

> STRONG & EMPHASSIS:
  - `<strong>` this declares that the content has a strong importance.
  - example:
    - <p><strong>Beware:</strong> Pickpockets operate in this area.</p>
    - as you can see beware is strong `<p><strong>Beware:</strong> Pickpockets operate in this area.</p>`
    - `<em>` Indicates emphasis that subtly changes the meaning of a sentence.
    - example: <p>I <em>think</em> Ivy was the first</p>
    - `<p>I <em>think</em> Ivy was the first</p>`
    as you can see "think" is emphasised.

> QUOTATIONS:
  
  * `<blockquote>` is used for longer quotes that take up an entire paragraph.
  * example: 
    - `<blockquote cite="http://en.wikipedia.org/wiki/Winnie-the-pooh"><p>Did you ever stop to think, and forget to start again?</p></blockquote>`
    - `<q>` is the element used for shorter quotes
     - <p>As A.A. Milne said, <q>Some people talk to animals. Not man listen thouigh. Thats the problem.</q></p>
     - What that code will look like `<p>As A.A. Milne said, <q>Some people talk to animals. Not man listen thouigh. Thats the problem.</q></p>`

> ABBREVIATIONS & ACRONYMS: 
    
  * `<abbr>` is used for a abbreviation or acronym. A title attribute `<title>` used on the opening tag is used to specify the full term.
    - `<p><abbr title="Professor">Prof</abbr> Stephen Hawking is a theoretical physicist and cosmologist.</p>` 
    - <p><abbr title="Professor">Prof</abbr> Stephen Hawking is a theoretical physicist and cosmologist.</p>    

> CITATIONS & DEFINITIONS: 
  * `<cite>` Is the element you use when you're referencing a book, film or reaserch paper.
    - `<p><cite>A brief history of time</time> by Stephen Hawking has sold over ten million copies worldwide.</p>`
    - <p><cite>A brief history of time</time> by Stephen Hawking has sold over ten million copies worldwide.</p>
  * `<dfn>` The first time you explain some new terminology in a document, it is know as the defining instance of it
    - `<p>A <dfn>black hole</dfn> is a region of space from which nothing, not even light, can escape.</p>`
    - <p>A <dfn>black hole</dfn> is a region of space from which nothing, not even light, can escape.</p>

> AUTHOR DETAILS:
  * `<address>` this element has quite a specific use: to contain contact details for the author of the page
    - it can contain a physical address but it doesn't have to. For example it can contain a phone number or email address.
    -`<address><p><a href="mailto:homer@example.org">homer@example.org</a></p>`
    - <address><p><a href="mailto:homer@example.org">homer@example.org</a></p>

> CHANGE TO CONTENT:
  * `<ins> <del>` The `<ins>` element can show content that has been inserted into a document, while `<del>` shows the text that has been deleted from it.
    - `<p>It was the <del>worst</del> <ins>best</ins> idea she had ever.</p>`
    - <p>It was the <del>worst</del> <ins>best</ins> idea she had ever.</p>
  * `<s>` This element indicates that something is no longer accurate.
    - `<p>Laptop computer:</p>`
      `<p><s>Was $995</s></p>`
      `<p>Now only $375</p>`
    - <p>Laptop computer:</p>
      <p><s>Was $995</s></p>
      <p>Now only $375</p>  


## **CHAPTER 10**
### **INTRODUCING CSS**

> CSS ASSOCIATES SSTYLE RULES WITH HTML ELEAMENTS:
  * CSS works by associating rules with HTML elemnts. These rules govern how the content of specific elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
    - p {
      font-family: Arial;}
    - in that line of text the p is the selector and font-family: Arial; is the declaration.
> CSS PROPERTIES AFFECT HOW ELEMENTS ARE DISPLAYED
  - CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, seperated by a colon. You can specify several properties in one delcaration, each separated by a semi-colon.
    - h1, h2, h3{
      font-family: Arial;
      color: yellow
    }   
    - in that line of text the property is color and the value is the actual color rendered.

> CSS SELECTORS:
  * **Universal selector**: Applies to all elements in the document `*{}` targets all the elements on the page
  * **Type selector**: Matches element names h1,h2,h3 {} targets the `<h1>,<h2>`, and `<h3>` elements
  * **Class selector**: matches an element whose class attribute has a value that matches on specified after the period symbole `.note {}` targets any element whose class attribute has a value, `p.note {}` targets only the `<p>` elements whose class attribute has a value of note.
  * **Id selector**: Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol `#introduction{}` which targets the element whose id attribute has a value of introduction
  * **Child selector**: matches an element that is a direct child of another `li>a {}`, which targets any `<a>` elements that are children of `<li>`(but not anoter `<a>` element on the page).
  * **Descendant selector**: Matches an element that is a decendent of another specified element(not just a direct child of that element) `P a {}` targets any `<a>` elements that sit inside a `<p>` element, even if there are other elements nested between them
  * **Adjacent sibling selector**: matches an element that is th next sibling of another `h1+p {}` targets the firs `<p>` element after any `<h1>` element(but not other `<p>` elements).
  * **General sibling selector**: matches an element that is a sibling of another, although it does not have to be the directly preceding element `h1~p {}` if you had two `<p>` elements that are siblings of an `<h1>` element, this rule would apply to both.