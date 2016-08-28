## Text Formatting - Line Breaks and Paragraphs

### Understanding Paragraphs

At Github a paragraph is simply one or more consecutive lines of text, separated by one or more _blank lines_.  

A _blank line_ is any line that "_looks like a blank line_", regardless if it has no characters or if it is filled with spaces and/or tabs (or a mix of both). If the line "_looks like a blank line_", it will render by the GFM as a"_blank line_".

For instance, if you write:

     **This is 
     one single
     paragraph!**

You will get a single paragraph:

**This is 
one single
paragraph!**

But, if you write:

     **This is 
     one single
     paragraph!**
     
     **This is 
     another paragraph!**
     
You will get multiple paragraphs:

**This is 
one single
paragraph!**
     
**This is 
another paragraph!**

*IMPORTANT:*  
The _formatting elements_ won't translate from one paragraph to another. It means if you add a _paragraph break_ without any regard to the _formatting elements_, you will get a "_broken_" **Markdown** result.

Here is an example:

     **This is one single paragraph 
     in bold! 
     
     This is another paragraph 
     that should also be in bold!**
     
You will get:

**This is one single paragraph 
in bold! 
     
This is another paragraph 
that should also be in bold!**
     
It happened because the bold element \*\* was not rendered, thus it got expopsed. To prevent such problems, make sure you properly close the _formatting elements_ if they are to existe allthe way to the end of a paragraph. Example:

     **This is one single paragraph 
     in bold!**
     
     This is another paragraph 
     that should also be in bold!**
     
You will get:

**This is one single paragraph 
in bold**
     
This is another paragraph 
that should also be in bold!**


**Notice:** Subsequent _blak lines_ will not render as multiple blank lines, resulting in one single blank line.

- - -

### Understanding Line Breaks


The paragraph end, however, can be a little bit more _tricky_ to visualize. At Github, based on the description above, a paragraph is considered terminated when it is immediately followed by a "_blank line_", or by a line beginning with a **Markdown character**.

, or when it has two blank spaces as last characters (standard **Markdown**).

This concept can confuse some people, thus lets explore it a bit for a better undetstanding.

If your paragraph is written like this:

    **Line 1** (terminated with no spaces)
    **Line 2** (terminated with _two white-space_ characters)  
    **Line 3** (terminated with no spaces)
    **Line 4** (terminated with no spaces)

It shour render like this:

**Line 1** (terminated with no spaces)
**Line 2** (terminated with _two white-space_ characters)  
**Line 3** (terminated with no spaces)
**Line 4** (terminated with no spaces)

Notice how a _line break_ was enforced in between the lines **2** and **3**. It was result of the two _blank space_  characters added to the end of the lines **2**. 

Originally Github didn't recognize this feature (which was defined in the **Markdown Standard**), but support for it has been added so Github would recognize and properly render _Markdown files_ created by other editors. 

At Github _line break_ and _new paragraph_ concepts can be deceiving, but it is important to know the semantical differences if you want to write proper documentation. You can always separate two paragraphs in Github by adding a _blank line_ in between them, knowingly that those ARE to be interpreted as **two separated paragraphs**. I fyou want, instead, keep the semantical interpretation of a paragraph but break lines inside it, then you must terminater the line(s) with  _two white-space_ characters to enforce a correct _line break_.

Technically is the same as use <code>&lt;p&gt;</code> and <code>&lt;p \\&gt;</code> in HTML.

fundamentally to get the same visual effect the _two white-space_ characters at the end of the paragraph 




Github itself will render a _line break_ in a paragraph is simply one or more consecutive lines of text, separated by one or more blank lines.




.) Normal paragraphs should not be indented with spaces or tabs.

The implication of the "one or more consecutive lines of text" rule is that Markdown supports "hard-wrapped" text paragraphs. This differs significantly from most other text-to-HTML formatters (including Movable Type's "Convert Line Breaks" option) which translate every line break character in a paragraph into a <br /> tag.

When you do want to insert a <br /> break tag using Markdown, you end a line with two or more spaces, then type return.

Yes, this takes a tad more effort to create a <br />, but a simplistic "every line break is a <br />" rule wouldn't work for Markdown. Markdown's email-style blockquoting and multi-paragraph list items work best -- and look better -- when you format them with hard breaks.

      

fvafvbadfsv
adfbadfvb

   dsfvbadfvadfvb
   adfvbadfv
   
      asdfvafdsv
      adsfvafdsv


Currently GitLab renders line-breaks in markdown files as line-breaks. We propose to change this behaviour to conform to the markdown specification and only render line-breaks when you end a line with two or more spaces. Paragraphs will continue to be rendered as before; when the text is separated by one or more blank lines.

The above change will ensure that markdown files in projects will look the way you expect them to look. But GitLab has just one markdown engine to render GitLab Flavored Markdown. Since descriptions & comments in both issues & merge requests also use GitLab Flavored Markdown they will also show the new behaviour. We think this is preferable above introducing different behaviour and rendering code for different cases. Please let us know what you think.




Traditional Markdown requires a two-space to generate line breaks, while GFM line breaks are automatically generated wherever you add a line break on your text. 

If you press <code>enter</code>


Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a separate paragraph.

This line is also begins a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the same paragraph.

(Technical note: Markdown Here uses GFM line breaks, so there's no need to use MD's two-space line breaks.)
Description


<table width="100%" valign="top" style='border: none;'>
<thead>
<tr>
  <td width="20%" nowrap>Markdown</td>
  <td width="20%" nowrap>Will Render As</td>
  <td width="0%">Notes & References</td>
</tr>
</thead>
<tbody>
<tr>
  <td width="20%" valign="top" nowrap><code>Markdown</code></td>
  <td width="20%" valign="top" nowrap>Sample</td>
  <td width="0%" valign="top">
      Notes about the Markdown (if any)
  </td>
</tr>
</tbody>
</table>

Reference Notes (if any)

[🔙 Back to the **General Index**](README.md#general-index)

- - - 
<sup>
<i>Except where otherwise noted, content on this document is licensed under a <b>Creative Commons Attribution 4.0</b> International license</i>.<br />
Provided by <b>Julio Marchi</b>
</sup>
