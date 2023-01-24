**Basic writing and formatting syntax**
Create sophisticated formatting for your prose and code on GitHub with simple syntax.

## Headings
To create a heading, add one to six # symbols before your heading text. The number of # you use will determine the size of the heading.

# The largest heading
## The second largest heading
###### The smallest heading
Rendered H1, H2, and H6 headings

When you use two or more headings, GitHub automatically generates a table of contents which you can access by clicking  within the file header. Each heading title is listed in the table of contents and you can click a title to navigate to the selected section.


## Styling text
You can indicate emphasis with bold, italic, strikethrough, subscript, or superscript text in comment fields and .md files.

Style	Syntax	Keyboard shortcut	Example	Output
Bold	** ** or __ __	Command+B (Mac) or Ctrl+B (Windows/Linux)	**This is bold text**	This is bold text
Italic	* * or _ _     	Command+I (Mac) or Ctrl+I (Windows/Linux)	*This text is italicized*	This text is italicized
Strikethrough	~~ ~~		~~This was mistaken text~~	This was mistaken text
Bold and nested italic	** ** and _ _		**This text is _extremely_ important**	This text is extremely important
All bold and italic	*** ***		***All this text is important***	All this text is important
Subscript	<sub> </sub>		<sub>This is a subscript text</sub>	This is a subscript text
Superscript	<sup> </sup>		<sup>This is a superscript text</sup>	This is a superscript text


## Quoting text
You can quote text with a >.

Text that is not a quote

> Text that is a quote

## Quoting code
You can call out code or a command within a sentence with single backticks. The text within the backticks will not be formatted. You can also press the Command+E (Mac) or Ctrl+E (Windows/Linux) keyboard shortcut to insert the backticks for a code block within a line of Markdown.

Use `git status` to list all new or modified files that haven't yet been committed.
`HIHIIHIHIHIH`

To format code or text into its own distinct block, use triple backticks.

Some basic Git commands are:
```
git status
git add
git commit
```
Rendered code block

For more information, see "Creating and highlighting code blocks."

If you are frequently editing code snippets and tables, you may benefit from enabling a fixed-width font in all comment fields on GitHub. For more information, see "Enabling fixed-width fonts in the editor."


##Supported color models

In issues, pull requests, and discussions, you can call out colors within a sentence by using backticks. A supported color model within backticks will display a visualization of the color.

The background color should be `#ffffff` for light mode and `#0d1117` for dark mode.
Rendered supported color model.

Here are the currently supported color models.

Color	Syntax	Example	Output
HEX	`#RRGGBB`	`#0969DA`	Rendered supported color model in HEX format.
RGB	`rgb(R,G,B)`	`rgb(9, 105, 218)`	Rendered supported color model in RGB format.
HSL	`hsl(H,S,L)`	`hsl(212, 92%, 45%)`	Rendered supported color model in HSL format.
Notes:

A supported color model cannot have any leading or trailing spaces within the backticks.
The visualization of the color is only supported in issues, pull requests, and discussions.

## Links
You can create an inline link by wrapping link text in brackets [ ], and then wrapping the URL in parentheses ( ). You can also use the keyboard shortcut Command+K to create a link. When you have text selected, you can paste a URL from your clipboard to automatically create a link from the selection.

You can also create a Markdown hyperlink by highlighting the text and using the keyboard shortcut Command+V. If you'd like to replace the text with the link, use the keyboard shortcut Command+Shift+V.

This site was built using [GitHub Pages](https://pages.github.com/).

Rendered link

Tip: GitHub automatically creates links when valid URLs are written in a comment. For more information, see "Autolinked references and URLs."

Section links
You can link directly to a section in a rendered file by hovering over the section heading to expose the link:

Section link within the README file for the github/scientist repository


## Relative links
You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:

[Contribution guidelines for this project](docs/CONTRIBUTING.md)
GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. The path of the link will be relative to the current file. Links starting with / will be relative to the repository root. You can use all relative link operands, such as ./ and ../.

Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.

Images
You can display an image by adding ! and wrapping the alt text in [ ]. Then wrap the link for the image in parentheses ().

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

Rendered Image

GitHub supports embedding images into your issues, pull requests, discussions, comments and .md files. You can display an image from your repository, add a link to an online image, or upload an image. For more information, see "Uploading assets."

Tip: When you want to display an image which is in your repository, you should use relative links instead of absolute links.

Here are some examples for using relative links to display an image.

Context	Relative Link
In a .md file on the same branch	/assets/images/electrocat.png
In a .md file on another branch	/../main/assets/images/electrocat.png
In issues, pull requests and comments of the repository	../blob/main/assets/images/electrocat.png?raw=true
In a .md file in another repository	/../../../../github/docs/blob/main/assets/images/electrocat.png
In issues, pull requests and comments of another repository	../../../github/docs/blob/main/assets/images/electrocat.png?raw=true
Note: The last two relative links in the table above will work for images in a private repository only if the viewer has at least read access to the private repository which contains these images.

For more information, see "Relative Links."

## Lists
You can make an unordered list by preceding one or more lines of text with -, *, or +.

- George Washington
* John Adams
+ Thomas Jefferson
Rendered unordered list

To order your list, precede each line with a number.

1. James Madison
2. James Monroe
3. John Quincy Adams
Rendered ordered list

## Nested Lists
You can create a nested list by indenting one or more list items below another item.

To create a nested list using the web editor on GitHub or a text editor that uses a monospaced font, like Visual Studio Code, you can align your list visually. Type space characters in front of your nested list item, until the list marker character (- or *) lies directly below the first character of the text in the item above it.

1. First list item
   - First nested list item
     - Second nested list item
Note: In the web-based editor, you can indent or dedent one or more lines of text by first highlighting the desired lines and then using Tab or Shift+Tab respectively.

Nested list with alignment highlighted

List with two levels of nested items

To create a nested list in the comment editor on GitHub, which doesn't use a monospaced font, you can look at the list item immediately above the nested list and count the number of characters that appear before the content of the item. Then type that number of space characters in front of the nested list item.

In this example, you could add a nested list item under the list item 100. First list item by indenting the nested list item a minimum of five spaces, since there are five characters (100. ) before First list item.

100. First list item
     - First nested list item
List with a nested list item

You can create multiple levels of nested lists using the same method. For example, because the first nested list item has seven characters (␣␣␣␣␣-␣) before the nested list content First nested list item, you would need to indent the second nested list item by seven spaces.

100. First list item
     - First nested list item
       - Second nested list item
List with two levels of nested items

For more examples, see the GitHub Flavored Markdown Spec.

## Paragraphs
You can create a new paragraph by leaving a blank line between lines of text.




# Organizing information with tables
In this article
## Creating a table
Formatting content within your table
Further reading
You can build tables to organize information in comments, issues, pull requests, and wikis.

Creating a table
You can create tables with pipes | and hyphens -. Hyphens are used to create each column's header, while pipes separate each column. You must include a blank line before your table in order for it to correctly render.


| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
Rendered table

The pipes on either end of the table are optional.

Cells can vary in width and do not need to be perfectly aligned within columns. There must be at least three hyphens in each column of the header row.

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |
Rendered table with varied cell width

If you are frequently editing code snippets and tables, you may benefit from enabling a fixed-width font in all comment fields on GitHub. For more information, see "Enabling fixed-width fonts in the editor."

## Formatting content within your table
You can use formatting such as links, inline code blocks, and text styling within your table:

| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |
Rendered table with formatted text

You can align text to the left, right, or center of a column by including colons : to the left, right, or on both sides of the hyphens within the header row.

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |
Rendered table with left, center, and right text alignment

To include a pipe | as content within your cell, use a \ before the pipe:

| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |
Rendered table with an escaped pipe


Organizing information with collapsed sections
In this article
Creating a collapsed section
Further reading
You can streamline your Markdown by creating a collapsed section with the `<details>` tag.

## Creating a collapsed section
You can temporarily obscure sections of your Markdown by creating a collapsed section that the reader can choose to expand. For example, when you want to include technical details in an issue comment that may not be relevant or interesting to every reader, you can put those details in a collapsed section.

Any Markdown within the `<details>` block will be collapsed until the reader clicks  to expand the details. Within the `<details>` block, use the `<summary>` tag to create a label to the right of .

```
<details><summary>CLICK ME</summary>
<p>

#### We can hide anything

</p>
</details>
```

The Markdown will be collapsed by default.

After a reader clicks , the details are expanded.

<details><summary>CLICK ME</summary>
<p>

#### We can hide anything, even code!

```
 "Hello World"
```

</p>
</details>


## Autolinked references and URLs
In this article
URLs
Issues and pull requests
Labels
Commit SHAs
Custom autolinks to external resources
Further reading
References to URLs, issues, pull requests, and commits are automatically shortened and converted into links.

URLs
GitHub automatically creates links from standard URLs.

Visit https://github.com

Rendered autolinked URL


**There are a lot more features to formatting, refer the below link for more GitHub Documentation**
Visit https://docs.github.com/en

