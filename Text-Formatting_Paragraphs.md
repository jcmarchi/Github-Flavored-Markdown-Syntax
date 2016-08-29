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
Most _formatting elements_ won't translate from one paragraph to another. It means if you add a _paragraph break_ without any regarding to the _formatting elements_, you may get a "_broken_" **Markdown** result.

Here is an example:

     **This is one single paragraph 
     in bold! 
     
     This is another paragraph 
     that should also be in bold!**
     
You will get it _broken_ like this:

**This is one single paragraph 
in bold! 
     
This is another paragraph 
that should also be in bold!**
     
As you can see the paragraph was rendered correctly but not the bold element (<code>\*\*</code>), which got exposed. To prevent such problem, make sure you properly close the _formatting elements_ if they are to exist all the way to the end of the paragraph.

Here how it is done right:

     **This is one single paragraph 
     in bold!**
     
     **This is another paragraph 
     that should also be in bold!**
     
So it can render correctly:

**This is one single paragraph 
in bold!**

**This is another paragraph 
that should also be in bold!**

**Notice:** Multiple _blak lines_ will render as a single blank line (like HTML).

- - -

### Understanding Line Breaks

Different from a paragraph, a _line break_ should simply do what it says: "**_break the line_**", not the paragraph.

If visually it can be identified by the lack of space (_blank lines_) in between the lines, semantically it means a lot more, allowing electronic readers, parsers and conversion tools to better understand where a paragraph begin and end.
  
This concept can be confused, so lets try some examples for a better understanding.

If your write a multi-line paragraph like this:

    **Line 1** (terminated with no spaces)
    **Line 2** (terminated with _two white-space_ characters)  
    **Line 3** (terminated with no spaces)
    **Line 4** (terminated with no spaces)

It will render like this:

**Line 1** (terminated with no spaces)
**Line 2** (terminated with _two white-space_ characters)  
**Line 3** (terminated with no spaces)
**Line 4** (terminated with no spaces)

Notice how a _line break_ was **ONLY** enforced in between the lines **2** and **3**, despite of how you actually wrote it. The _line breaker_ enforcer are the two _blank space_ characters that exist at the end of the lines **2**. 

Originally, Github didn't recognize this feature (defined by the **Markdown Standard**), but support for it has been added so Github would recognize and properly render _Markdown files_ created by other editors. I agree a better choice could have been made other than something "invisible" to the eye, but it is what it is...

**Important:** An empty paragraph terinated in two _blank space_ characters will stil be rendered as a _blank line_ because it "_looks like a blank line_" (se description of paragraph above).


- - - 

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
