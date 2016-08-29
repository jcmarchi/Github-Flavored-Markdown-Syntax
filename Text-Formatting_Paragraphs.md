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

### Multiple _Blank Lines_ in Github Markdown

After reading and experiencing with paragraphs and _line breaks_ a common question rises: _How to create more than one subsequent **blank line** in between paragraphs?_

Well, without _tricking_ the GFM it is not exactly doable, but you can always try those options:

1. Use the HTML Tag <code>&lt;br \\&gt;</code> to force a _line break_ 
2. Use the _blank space_" character (<code>\&nbsp;</code>) to force a _blank line_, one per line, and having the line terminated by _two blank spaces_,.
 
Here the examples (pay good attention to it):

#### Option 1: Using <code>&lt;br \\&gt;</code> to force a _line break_:

    Line 1
    
    <br /><br /><br />
    Line 2
    <br />
    Line 3

Will render as:

Line 1

<br /><br /><br />
Line 2
<br />
Line 3

#### Option 2: Using the _blank space_" character (<code>\&nbsp;</code>):

        Line 1
        
        &nbsp;  
        &nbsp;  
        &nbsp;  
        Line 2
        &nbsp;  
        Line 3

Will render as:

Line 1

&nbsp;  
&nbsp;  
&nbsp;  
Line 2
&nbsp;  
Line 3

Notice that both examples above have their first _blank line_ as a real _blank line_. Without it you will always have the first _force blank line_ added to the end of the previous line (unless if it is terminated with _two blank spaces_). Well, you got it! Right? :)


[🔙 Back to the **General Index**](README.md#general-index)

- - - 
<sup>
<i>Except where otherwise noted, content on this document is licensed under a <b>Creative Commons Attribution 4.0</b> International license</i>.<br />
Provided by <b>Julio Marchi</b>
</sup>
