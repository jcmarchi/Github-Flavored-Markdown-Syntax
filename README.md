# Github Flavored Markdown Syntax #
_The unofficial cheat sheet for the **.md** files_
------

GitHub uses its own unique render to display **.md** files in your Internet Browser of choice. Commonly known as "GitHub Flavored Markdown," or GFM, it is used across the system to render **.md** files (A.K.A. "_documents_"), whikch are used in wiki pgaes, projects documens, issues, comments, and pull requests. 

The GFM rendering process differs from Standard Markdown (SM) in a few significant ways. It also adds few key functionalities and adjust the render tailoring it for Github usage purposes. You can lear more about it at <a href="https://github.com/github/markup#markups" target="_blank">Github Markups</a>. 

If you're not already familiar with **Markdown**, take a look at some **Markdown Basics** (<a href="https://www.google.com/#newwindow=1&safe=off&q=%22Markdown+Basics%22+tutorials" target="_blank">search for it on Google</a>), there are great tutorials available). Just remember Github's GFM has extra features that are tailored for its own needs, such as: pull request integration, SHA-1 Conversion (see below), task lists and more.

An important remark for anyone writing documentation inside Github projects: the GFM render accepts a handfull of **HTML TAGS** (HTML 4.1) and render them properly, applying to the resultant page the same _styling_ (CSS) the referenced Markdown element wold receive. In certain cases you can even add some extra styling (CSS) to your tags and, as far as it won't conflict with Github's CSS, it should render correctly too. So, few free to use markup, HTML Tags or both at same time. Try it, and see for yourself. Sure enought you will find situations in which HTML TAGS (with or without styling) will better serve some purposes than the referenced Markdown element and vice-versa. 

Express your freedom and have a great writting experience.

## Text Formatting Markdown ##

<table style='border: none' width="100%" v-align="top">
<tr>
  <td width="20%" nowrap>Markdown</td>
  <td width="20%" nowrap>Will Render As</td>
  <td width="0%">Notes & References</td>
</tr>
<tr>
  <td width="20%" nowrap><code># Heading 1 #</code></td>
  <td width="20%" nowrap><h1>Heading 1</h1></td>
  <td width="0%">
      Equivalent to <code><b>&lt;h1&gt;</b></code> tag, but with a thin <i>horizontal underline</i> attached.<br /><br />
      Same effect can be obtained by adding <code>===</code> as the very next paragraph.
  </td>
</tr>
<tr>
  <td width="20%" nowrap><code>## Heading 2 ##</code></td>
  <td width="20%" nowrap><h2>Heading 2</h2></td>
  <td width="0%">
      Equivalent to <code><b>&lt;h2&gt;</b></code> tag, but with a thin <i>horizontal underline</i> attached.<br /><br />
      Same effect can be obtained by adding <code>---</code> as the very next paragraph.
  </td>
</tr>
<tr>
  <td width="20%" nowrap><code>### Heading 3 ###</code></td>
  <td width="20%" nowrap><h3>Heading 3</h3></td>
  <td width="0%">Equivalent to <code><b>&lt;h3&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" nowrap><code>#### Heading 4 ####</code></td>
  <td width="20%" nowrap><h4>Heading 4</h4></td>
  <td width="0%">Equivalent to <code><b>&lt;h4&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" nowrap><code>##### Heading 5 #####</code></td>
  <td width="20%" nowrap><h5>Heading 5</h5></td>
  <td width="0%">Equivalent to <code><b>&lt;h5&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" nowrap><code>###### Heading 6 ######</code></td>
  <td width="20%" nowrap><h6>Heading 6</h6></td>
  <td width="0%">Equivalent to <code><b>&lt;h6&gt;</b></code> tag.</td>
</tr>
</table>
