# Github Flavored Markdown Syntax
_The unofficial cheat sheet for the **.md** files_
------

Github uses its own version of **Markdown** to interpret and parse (**.md**) files, known as "GitHub Flavored Markdown" (GFM). It is available across the Github system wherever a _document_ is present: **wiki pages**, **project reference files** and **project descriptions**, **issues tracking**, **comments**, and **pull requests**. You can learn more about the GFM implementation at <a href="https://github.com/github/markup#markups" target="_blank">Github Markups</a>. 

If you're not yet familiar with **Markdown**, take a look at some **Markdown Basics** (<a href="https://www.google.com/#newwindow=1&safe=off&q=%22Markdown+Basics%22+tutorials" target="_blank">search for it on Google</a>). There are great tutorials available. By knowing the basics about **Markdown** it will make a lot more sense why the GFM rendering process differs from the <a href="http://daringfireball.net/projects/markdown/" target="_blank">**Standard Markdown**</a>. Fundamentally, the GFM is tailored for Github to allow the _documents_ to serve to a higher purposed within Github scope other than simply disclose information. The GFM adds _key functionalities_ such as: **pull request integration**, **SHA-1 Conversion**, **task lists**, **emoji**, **named anchors**, **CDN caching for images**, **autolinking** etc. 

An important remark for anyone writing documentation inside Github projects: the GFM render also accepts a handfull of **HTML TAGS** and render them properly, but not before **aggressively sanitize** them to remove things such as: **scripts tags**, (_some_) **inline-styles**, **classes** and **id attributes**. You can take a look at the <a href="https://github.com/rgrove/sanitize/#readme" target="_blank">sanitization filter</a> for the full whitelisted HTML.

My recommendation for anyone trying to make the best out of the GFM is to fell free to use **Markdown**, **HTML Tags** or **_both_** at same time. Try it and see for yourself. Sure enough you will find situations in which **HTML Tags** will be much better fit than the equivalent **Markdown** element and vice-versa (this entire set of documents are great example of such combination).

Express your freedom, fell free to learn from this set of documents and have a great writting experience. That's exactly _why_ I decided to make it as a set of **.md** files instead of a Wiki page.

Have fun.

[**Julio Marchi ©**](mailto:jcmarchi@gmail.com) &nbsp; 😎 <br />
<sup>Twitter: <a href="https://twitter.com/MrMarchi">@MrMarchi</a></sup>

- - - 

## General Index

### Text Formatting
* Line Breaks (concept)
* [Headers](Text-Formatting_Headers.md)
* Content Elements (Bold, Italic, Strikethrough, etc.)
* Unicode Characters and HTML entities

### Blocks Structures
* Lists (Ordered and Unordered)
* Tables
* Horizontal Rule

### Links & References
* Images
* Links & Anchors
* Videos

### Advanced or Exclusive GFM Formatting
* Code Syntax Highlighting
* Task Lists
* SHA references
* Issue references within a repository
* Emoji

