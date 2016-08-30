## Text Formatting - Headers

<kbd>CTRL</kbd>+<kbd>Z</kbd>
Primarily used to visually and semantically identify contents and defined contexts, such as **titles**, **topics** and **sub-topics**.

The **Header Markdow** character (<code>**#**</code>) must be the first element of the line, otherwise it will simply render the _hash_ symbol (<code>**#**</code>). As result, it is not possible to use it inside a paragraphs to obtain the same visual format.

If, for any reason, your text required the _hash_ symbol (<code>**#**</code>) appearing as the first character of a line, it is possible to _escape_ it by preceding it with the _backslash-escape_ character <code>**\**</code>. E.g.: <code>\\# Will not render as a header element</code>.


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
  <td width="20%" valign="top" nowrap>
      <code># Heading 1</code> <br /><br />
      <sub>Alternative Formatting Option:</sub> <br /><br />
      <code>Heading 1</code> <br />
      <code>===</code>
  </td>
  <td width="20%" valign="top" nowrap><h1>Heading 1</h1></td>
  <td width="0%" valign="top">
      Equivalent to <code><b>&lt;h1&gt;</b></code> tag, but with a thin <i>horizontal underline</i> attached.<br /><br />
      Same effect can be obtained by adding <code>===</code> as the very next paragraph.
  </td>
</tr>
<tr>
  <td width="20%" valign="top" nowrap>
      <code>## Heading 2</code> <br /><br />
      <sub>Alternative Formatting Option:</sub> <br /><br />
      <code>Heading 2</code> <br />
      <code>---</code>
  </td>
  <td width="20%" valign="top" nowrap><h2>Heading 2</h2></td>
  <td width="0%" valign="top">
      Equivalent to <code><b>&lt;h2&gt;</b></code> tag, but with a thin <i>horizontal underline</i> attached.<br /><br />
      Same effect can be obtained by adding <code>---</code> as the very next paragraph.
  </td>
</tr>
<tr>
  <td width="20%" nowrap><code>### Heading 3</code></td>
  <td width="20%" nowrap><h3>Heading 3</h3></td>
  <td width="0%">Equivalent to <code><b>&lt;h3&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" nowrap><code>#### Heading 4</code></td>
  <td width="20%" nowrap><h4>Heading 4</h4></td>
  <td width="0%">Equivalent to <code><b>&lt;h4&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" nowrap><code>##### Heading 5</code></td>
  <td width="20%" nowrap><h5>Heading 5</h5></td>
  <td width="0%">Equivalent to <code><b>&lt;h5&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" nowrap><code>###### Heading 6</code></td>
  <td width="20%" nowrap><h6>Heading 6</h6></td>
  <td width="0%">Equivalent to <code><b>&lt;h6&gt;</b></code> tag.</td>
</tr>
</tbody>
</table>

As an interesting remark, you can use the equivalent **Markdown Syntax** of <code># Heading 1</code> and/or <code>## Heading 2</code> to create [Horizontal Rules](Blocks-Structures_HorizontalRule.md).

[:arrow_left: Back to the **General Index**](README.md#general-index)

- - - 
<sup>
<i>Except where otherwise noted, content on this document is licensed under a <b>Creative Commons Attribution 4.0</b> International license</i>.<br />
Provided by <b>Julio Marchi <sup>©</sup></b>
</sup>
