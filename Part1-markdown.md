# Introduction to Markdown

Markdown is a lightweight markup language with plain text formatting syntax. What this means to you is that by using just a few extra symbols in your text, Markdown helps you create a document with an explicit structure.

## Why Markdown

* **Easy** The syntax is very simple.

* **Fast:**  It speeds up the workflows.

* **Clean:** No missing closing tags, no improperly nested tags, no blocks left without containers.

* **Portable:**  Cross-platform by nature.

* **Flexible:** Output documents to a wide array of formats like, convert to HTML , rich text for sending emails or any number of other proprietary formats.


> We will be using markdown in almost every module's assignment, so it is an important thing learn here if you don't know already.

## Basic working in Markdown

### <u>1. Heading</u>

Use # for headings. You can use this like in HTML for H1, H2 etc.

<ins>

**Input:**

</ins>

```md

# H1
## H2
### H3
.
.
###### H6
```

**<ins>Output:</ins>**

# H1
## H2
### H3
.

.
###### H6

<hr>

### 2. Bold and Italics

Use `**` for making text bold and `*` for italics.

> You are required to close the tag here.

**<ins>Input:</ins>**

```md

**Bold**
*Italics*
***Bold and Italics Both***

```

**<ins>Output:</ins>**

**Bold**

*Italics*

***Bold and Italics Both***


<hr>

### 3. Lists

Use `*` from new line for unordered list, `1.` for order.

>  You can also use these with proper indentation.

**<ins>Input:</ins>**

```md

* Unordered

1. Ordered

* Nested
   1. ordered inside.
      * Unordered inside

```

**<ins>Output:</ins>**


* Unordered

1. Ordered

* Nested
   1. ordered inside.
      * Unordered inside
      


<hr>

### 4. Hyperlinks and images

Use `[text](url)` for hyperlinks and, `![text](path/url)` for image.

>  You can also use image links by nesting these both.

**<ins>Input:</ins>**

```md

[Devincept Website](https://devincept.tech/)

![DevIncept logo image](extras/logo.gif)

[![DevIncept logo image link](extras/logo.gif)](https://devincept.tech/)

```

**<ins>Output:</ins>**

[Devincept Website](https://devincept.tech/)

![DevIncept logo image](extras/logo.gif)

[![DevIncept logo image link](extras/logo.gif)](https://devincept.tech/)

      
