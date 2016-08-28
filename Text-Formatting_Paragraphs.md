## Text Formatting - Line Breaks and Paragraphs

Currently GitLab renders line-breaks in markdown files as line-breaks. We propose to change this behaviour to conform to the markdown specification and only render line-breaks when you end a line with two or more spaces. Paragraphs will continue to be rendered as before; when the text is separated by one or more blank lines.

The above change will ensure that markdown files in projects will look the way you expect them to look. But GitLab has just one markdown engine to render GitLab Flavored Markdown. Since descriptions & comments in both issues & merge requests also use GitLab Flavored Markdown they will also show the new behaviour. We think this is preferable above introducing different behaviour and rendering code for different cases. Please let us know what you think.




A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. (A blank line is any line that looks like a blank line -- a line containing nothing but spaces or tabs is considered blank.) Normal paragraphs should not be indented with spaces or tabs.

The implication of the "one or more consecutive lines of text" rule is that Markdown supports "hard-wrapped" text paragraphs. This differs significantly from most other text-to-HTML formatters (including Movable Type's "Convert Line Breaks" option) which translate every line break character in a paragraph into a <br /> tag.

When you do want to insert a <br /> break tag using Markdown, you end a line with two or more spaces, then type return.

Yes, this takes a tad more effort to create a <br />, but a simplistic "every line break is a <br />" rule wouldn't work for Markdown. Markdown's email-style blockquoting and multi-paragraph list items work best -- and look better -- when you format them with hard breaks.


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
