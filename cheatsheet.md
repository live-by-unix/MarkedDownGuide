## Markdown cheatsheet
**Covers everything in guide.md**
The follwing is included:
* Headings
* Lists
* Links
* Fenced code blocks
* Block Quotes
* Images
* Tables
* Strikethrough
* Emoji support

### Headings
The six heading levels are:
```markdown
# Heading Level 1 (Main Title / <h1>)
## Heading Level 2 (Major Section / <h2>)
### Heading Level 3 (Subsection / <h3>)
#### Heading Level 4 (Sub-subsection / <h4>)
##### Heading Level 5 (Rarely Used / <h5>)
###### Heading Level 6 (Smallest / <h6>)
``` 
These are the common ways to use the different headings. But of course, you can use them in different ways.   

### Lists

#### Unordered lists
These are lists which are like unordered bullet points in GDocs.          
You can use `-` (hyphens) , `+` (plus) , or `*`(asterisk)
For example:    
* This
* is
* a
* list

- This
- is
- a
- list

and     
+ This
+ is
+ a
+ list

The one I like the best are asterisks.    

### Ordered lists
Basic ordered lists:
```markdown
1. This
2. Is
3. Basic
```
That list is easily to make. Put a number, then a period next to it, then a space, then your word.      
So that should render as:
1. This
2. Is
3. Basic
Most parsers just put the next number after the return for you.   

Nested ordered lists:
```markdown
1. Fruits
    1. Apple
    2. Banana
2. Vegetables
    1. Carrot
    2. Lettuce
```
That would render as:   
1. Fruits
    1. Apple
    2. Banana
2. Vegetables
    1. Carrot
    2. Lettuce

  You would create the same 1. as a ordered list, then return, then `tab`, then put the same 1. as a ordered list.     
  Again, most editors automatically put the next number in the list.     

<div style="max-width:900px; margin:auto;">
    <iframe 
        src="https://marky-editor.pages.dev"
        style="width:100%; height:600px; border:none;">
    </iframe>
</div>


  ### Links
  Links are ways to lead to a webpage directly in your markdown.    
  
  You can put the link directly, but if you a word for the user to click that leads to the link (a hyperlink), do this syntax.   
  ```markdown
[Leads to example.com](https://www.example.com)
```
The `[]` is the place where you put the word, and the `()` is where you put link.   

In total, it would render like:
[Leads to example.com](https://www.example.com)

By default, Markdown will open the link & highlight it if you just put the link directly.      
But to be sure, put the link in the `[]` and the link AGAIN in the `()` to make the link as a "word" which leads to the link.    

### Fenced code blocks
We don't teach normal code blocks, as fenced code blocks are:  
* Easier to use in lists
* More used
* The standard in Markdown
* **And more reasons!**

To make a fenced code block, do this.      
Put 3 backticks (`) and then the word of your programming language.       

So ```perl or ```html or ```markdown or anything really, just double check it is valid by markdown standards.   
Then create a new line, and put the code you need.     
Then create a newline and put 3 more backticks.   
So if I needed to share a python snippet, I would do this:

````markdown
```python
def hello_world():
    print("Hello, World!")
```
````
If you need to put a fenced code block inside of a code block, just put more backticks then the fenced code block you are trying to put in the fenced code block.    
Make sure to still include the language name in both the code blocks!     

### Block Quotes
To make a block quote, do this:  
```markdown
> This is a block quote.
```
It would render as:  
> This is a block quote.

### Images
To put images do this:
```markdown
![Alt text](image.png)
```
If you want to put a image from the web, do this:
```markdown
![OpenAI Logo](https://images.ctfassets.net/kftzwdyauwt9/2fkAIT3PbTRytKTBx9cx8o/229bc28cb338565fe735d8935abc801f/OpenAI_Wordmark_Gif.gif?w=1920&q=90&fm=webp)
```
If you want to put text as description along side the of the image do this:
```markdown
![OpenAI Logo](https://images.ctfassets.net/kftzwdyauwt9/2fkAIT3PbTRytKTBx9cx8o/229bc28cb338565fe735d8935abc801f/OpenAI_Wordmark_Gif.gif?w=1920&q=90&fm=webp "GIF of OpenAI logo")
```
You can do the same with images from your host. 
**You can do even more with images!**

<div style="max-width:900px; margin:auto;">
    <iframe 
        src="https://marky-editor.pages.dev"
        style="width:100%; height:600px; border:none;">
    </iframe>
</div>

### Tables
To do tables do this:
```markdown
| Name  | Age | City      |
|-------|-----|-----------|
| Alice | 25  | New York  |
| Bob   | 30  | London    |
| Carol | 28  | Tokyo     |
```
That would render as:

| Name  | Age | City      |
|-------|-----|-----------|
| Alice | 25  | New York  |
| Bob   | 30  | London    |
| Carol | 28  | Tokyo     |

The table is created using pipes `|` and hyphens `-`
To align, do this:
```markdown
| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| Apple      | Banana       | 10          |
| Orange     | Grape        | 20          |
```
Notice the semicolons! It would render as:   

| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| Apple      | Banana       | 10          |
| Orange     | Grape        | 20          |

### Strikethrough
This is to cross out words.  
You can do this with markdown like this:
```markdown
~~Hello, World!~~
```
It would render as
~~Hello, World!~~
You can use these in sentences, font styling (coming up), anywhere with words.     

### Font styling
This is a table on how to do font styling: 
| Style         | Markdown                     | Result     |
| ------------- | ---------------------------- | ---------- |
| Italic        | `*text*` or `_text_`         | *text*     |
| Bold          | `**text**` or `__text__`     | **text**   |
| Bold + Italic | `***text***` or `___text___` | ***text*** |
| Strikethrough | `~~text~~`                   | ~~text~~   |
| Inline Code   | `` `text` ``                 | `text`     |

### Emoji support
Emojis happen when you put two semicolons: `::`    
Then put the emoji name in between those two semicolons, so for this emoji: 😃, you would do:       
 
```markdown
:smiley:
```
Check the specific names & see if your markdown has it before using.     

## Practice
To practice, I have listed some activities below:
* Trying to make a README.md for a GitHub project
* Rewriting your HTML file's code as much as you can into Markdown
* Trying to write guides like this in Markdown
* **And learning more!** (It never hurts)

## Parsers
Web Parsers:
| Parser          | Language   | Features                                                  |
| --------------- | ---------- | --------------------------------------------------------- |
| **Marked**      | JavaScript | Fast, lightweight, GitHub-Flavored Markdown (GFM) support |
| **markdown-it** | JavaScript | Highly extensible with plugins                            |
| **Micromark**   | JavaScript | CommonMark-compliant, powers the unified ecosystem        |
| **Remark**      | JavaScript | Parse, transform, and render Markdown using plugins       |
| **Showdown**    | JavaScript | Converts Markdown ↔ HTML                                  |
| **Snarkdown**   | JavaScript | Tiny (~2 KB), minimal parser                              |

Mobile Parsers:
* Markwon (Android) (Kotlin/Java)
* Down (Swift, iOS)
* Ink (Swift, iOS)

Desktop Parsers:
| Platform          | Popular Parsers                                          |
| ----------------- | -------------------------------------------------------- |
| **Electron**      | Marked, markdown-it, Micromark, Remark                   |
| **Tauri**         | pulldown-cmark (Rust), markdown-it (JavaScript frontend) |
| **Qt (C++)**      | cmark, MD4C                                              |
| **GTK (C/C++)**   | cmark, MD4C                                              |
| **.NET (C#)**     | Markdig                                                  |
| **Java**          | commonmark-java, flexmark-java                           |
| **Python**        | Mistune, Python-Markdown, Markdown2                      |
| **Swift (macOS)** | Down, Ink                                                |
| **Rust**          | pulldown-cmark, comrak                                   |
