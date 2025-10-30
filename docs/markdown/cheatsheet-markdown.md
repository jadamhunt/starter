# Headers and Breakpoints

# H1
## H2
### H3
#### H4
##### H5
###### H6

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

## Creating Breakpoints


Breakpoint created with `---` (*3 or more dashes*)

---

## Alternative Headings

You can create alternative headings by placing `---` or `===` under text:
```markdown
Alt-H1
---

Alt-H2
===
```

# Emphasizing Text
```
Italics - *text to emphasize* 
Alt. Italics - _text to emphasize_ 
Bold - **text to emphasize**
Strikethrough - ~~text to emphasize~~
```

Italics - *text to emphasize* \
Alt. Italics - _text to emphasize_ \
Bold - **text to emphasize** \
Strikethrough - ~~text to emphasize~~

# Listing and Bullets
```
1. First ordered list item
2. Another item
⋅⋅⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses
```

1. First ordered list item
2. Another item
    * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
    1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.
   Note that this line is separate, but within the same paragraph.  
   (This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

# Indexing and Links

## Inline links

This is text with a [link](https://youtu.be/dQw4w9WgXcQ?si=P4ekvanjT7UTDyS7).

```This is text with a [link](https://youtu.be/dQw4w9WgXcQ?si=P4ekvanjT7UTDyS7).```

This  [link](https://youtu.be/dQw4w9WgXcQ?si=P4ekvanjT7UTDyS7 "Never gonna give you up... :)") with a title.

```This  [link](https://youtu.be/dQw4w9WgXcQ?si=P4ekvanjT7UTDyS7 "Never gonna give you up... :)") with a title.```

## Relative Linking
Relative [links](./target_dir/ref_target.txt) 
```
Relative [links](./target_dir/ref_target.txt) 
```
These link to something relative to the path of the Markdown file, for example the target file is in another directory.

## Referencing Links

[Reference-style links][1]

[1]: https://www.google.com

Reference links keep your markdown clean and let ugly long links live anywhere in your file (*like the end*).
```
[Reference-style links][1]
[1]: https://www.google.com
```

## Empty Links

You can have empty links or [link within text] to itself.

[link within text]: https://www.hellokittyislandadventure.com/


## Images
Images can be linked directly via URL or relatively to a local file.
Additionally, you can add alt-text for screen readers (**please** do!), other modern features like hover-text are natively supported as well.

Inline local image ![alt text](steam_bg.png "hover text")

```markdown
Inline image ![alt text](steam_bg.png "hover text")
```
Remote image ![alt text](https://placehold.co/400x200 "Hosted image")
```markdown
Remote image ![alt text](https://placehold.co/400x200 "Hosted image")
```
A reference image: 

![penguin][ref_image]
```markdown
![penguin][ref_image]
... many lines later ...
[ref_image]: penguin.png
```

[ref_image]: penguin.png

# Code blocks

You can embed code with syntax highlighting.

First, in-line code: `aVar = "string saved to variable"` with single back-ticks "`"
```
First, in-line code: `aVar = "string saved to variable"`
```

Code blocks use 3 back-ticks "```":

```
# Python snippit
aVar = "new String"
aList = ["thing1", "thing2", "thing3"]
```

````
```
# Python snippit
aVar = "new String"
aList = ["thing1", "thing2", "thing3"]
```
````

Now, with language support, just add the language after the first backticks:
` ```python `

```python
# Python snippit
aVar = "new String"
aList = ["thing1", "thing2", "thing3"]
```

````
```python
# Python snippit
aVar = "new String"
aList = ["thing1", "thing2", "thing3"]
```
````



Let's look at some Python:


# Tables

I love **tables**

| Header | Data | Notes |
| :---: | --- | -----: |
| Set 1 | 33.4% | Expected result |
| Set 2 | 02.3% | Interesting... |
| Set 3 | 11.4% | I have *no idea* what I'm looking at |
| Set 4 | 5.62% | **Shiny!** numbers... |

```
| Header | Data | Notes |
| --- | :---: | ---: |
| Set 1 | 33.4% | Expected result |
| Set 2 | 02.3% | Interesting... |
| Set 3 | 11.4% | I have *no idea* what I'm looking at |
| Set 4 | 5.62% | **Shiny!** numbers... |
```

## Some table notes:

   *  One column must have **At least** 3 dashes `-` between header and data rows.  
  * Dashes *can* define ration of column width, depends on renderer.  
  * Regardless of how it looks when you type, it will still render *pretty*. No need to line up column lines.

  * Text in **columns** can be aligned with **colons**:
    * Left-adjusted `:---` or `---` *(default)*
    * Center-adjusted: `:-:`
    * Right-adjusted: `---:`

# Block Quotes

# HTML

# Markdown Tools

I love the **apostrophe** app for linux (flatpak)

For VScode, I use [Markdown Editor](https://youtu.be/dQw4w9WgXcQ?si=P4ekvanjT7UTDyS7 ) by *zaaack* \
and [Markdown PDF]( https://open-vsx.org/extension/yzane/markdown-pdf) by *yzane*


