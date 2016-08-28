# Github Flavored Markdown Syntax
_The unofficial cheat sheet for the **.md** files_
------

Github uses its own version of **Markdown** to interpret and parse (**.md**) files, known as "GitHub Flavored Markdown" (GFM). It is available across the Github system wherever a _document_ is present: **wiki pages**, **project reference files** and **project descriptions**, **issues tracking**, **comments**, and **pull requests**. You can learn more about the GFM implementation at <a href="https://github.com/github/markup#markups" target="_blank">Github Markups</a>. 

If you're not yet familiar with **Markdown**, take a look at some **Markdown Basics** (<a href="https://www.google.com/#newwindow=1&safe=off&q=%22Markdown+Basics%22+tutorials" target="_blank">search for it on Google</a>). By knowing the basics about **Markdown** it will make a lot more sense why the GFM rendering process differs from the <a href="http://daringfireball.net/projects/markdown/" target="_blank">**Standard Markdown**</a>. Fundamentally, the GFM is tailored for Github to allow the _documents_ to serve to a higher purposed within Github scope other than simply disclose information. The GFM adds _key functionalities_ such as: **pull request integration**, **SHA-1 Conversion**, **task lists**, **emoji**, **named anchors**, **CDN caching for images**, **autolinking** etc. 

An important remark for anyone writing documentation inside Github projects: the GFM render also accepts a handfull of **HTML TAGS** and render them properly, but not before **aggressively sanitize** them to remove things such as: **scripts tags**, (_some_) **inline-styles**, **classes** and **id attributes**. You can take a look at the <a href="https://github.com/rgrove/sanitize/#readme" target="_blank">sanitization filter</a> for the full whitelisted HTML.

My recommendation for anyone trying to make the best out of the GFM is to fell free to use **Markdown**, **HTML Tags** or **_both_** at same time. Try it and see for yourself. Sure enough you will find situations in which **HTML Tags** will be much better fit than the equivalent **Markdown** element and vice-versa (this entire set of documents are great example of such combination).

Express your freedom, fell free to learn from this set of documents and have a great writting experience. That's exactly _why_ I decided to make it as a set of **.md** files instead of a Wiki page.

Have fun.

[**Julio Marchi ©**](mailto:jcmarchi@gmail.com) &nbsp; 😎 <br />
<sup>Twitter: <a href="https://twitter.com/MrMarchi">@MrMarchi</a></sup>

- - - 

## General Index

### Text Formatting
* [Line Breaks and Paragraphs](Text-Formatting_Paragraphs.md)
* [Headers](Text-Formatting_Headers.md)
* [Content Elements (Bold, Italic, Strikethrough, etc.)](Text-Formatting_Content.md)
* [Unicode Characters and HTML entities](Text-Formatting_Unicode.md)

### Blocks Structures
* [Lists (Ordered and Unordered)](Blocks-Structures_Lists.md)
* [Tables](Blocks-Structures_Tables.md)
* [Horizontal Rule](Blocks-Structures_HorizontalRules.md)

### Links & References
* [Images](Links-and-References_Images.md)
* [Links & Anchors](Links-and-References_Links.md)
* [Videos](Links-and-References_Videos.md)

### Advanced or Exclusive GFM Formatting
* [Code Syntax Highlighting](Advanced-Exclusive_Highlight.md)
* [Task Lists](Advanced-Exclusive_TaskList.md)
* [SHA references](Advanced-Exclusive_SHA.md)
* [Issue references within a repository](Advanced-Exclusive_Issues.md)
* [Emoji](Advanced-Exclusive_Emoji.md)

- - - 
<sup>
<i>Except where otherwise noted, content on this document is licensed under a <b>Creative Commons Attribution 4.0</b> International license.</i><br />
Provided by <b>Julio Marchi</b>
</sup>
