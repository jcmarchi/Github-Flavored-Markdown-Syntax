# Github Flavored Markdown Syntax
_The unofficial cheat sheet for the **.md** files_
------

GitHub uses its own unique render to display **.md** files in your Internet Browser of choice. Commonly known as "GitHub Flavored Markdown," or GFM, it is used across the system to render **.md** files (A.K.A. "_documents_"), which are used in wiki pages, project documents, issues tracking, comments, and pull requests. 

The GFM rendering process differs from Standard Markdown (SM) in a few significant ways. It also adds few key functionalities and adjust the render tailoring it for Github usage purposes. You can lear more about it at <a href="https://github.com/github/markup#markups" target="_blank">Github Markups</a>. 

If you're not already familiar with **Markdown**, take a look at some **Markdown Basics** (<a href="https://www.google.com/#newwindow=1&safe=off&q=%22Markdown+Basics%22+tutorials" target="_blank">search for it on Google</a>), there are great tutorials available). Just remember Github's GFM has extra features that are tailored for its own needs, such as: pull request integration, SHA-1 Conversion (see below), task lists and more.

An important remark for anyone writing documentation inside Github projects: the GFM render recognizes a handfull of **HTML TAGS** and render them properly, but not before **aggressively sanitize** them, removing things such as: scripts tags, (some) inline-styles, classes and id attributes. You can take a look at the <a href="https://github.com/rgrove/sanitize/#readme" target="_blank">sanitization filter</a> for the full whitelisted HTML.

I would say you should fell free to use Markup, HTML Tags or both at same time. Try it and see for yourself. Sure enought you will find situations in which HTML TAGS will better fit than the equivalent Markdown and vice-versa.

Express your freedom and have a great writting experience.

## General Index [](#TOC)

### Text Formatting
* Line Breaks (concept)
* [Headers](Text-Formatting_Headers.md)
* Emphasis
 * Bold
 * Italic
* Strikethrough
* Highlighting


### Blocks Structures
* Lists
 * Unordered
 * Ordered
* Tables
* Horizontal Rule


### Links & References
* Images
* URL


### Advanced or Exclusive GFM Formatting
* Inline code
* Syntax highlighting
* Task Lists
* SHA references
* Issue references within a repository
* Emoji
