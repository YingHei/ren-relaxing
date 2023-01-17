---
title: "Basic Markdown"
date: 2023-01-13T23:13:23+08:00
draft: false
---

Markdown is very easy to learn and write. It is broadly used in websites, notes, documents, etc. 

In this article, we will go through some basic syntax of markdown to help you get started.

I strongly encourage you to take this [interactive tutorial](https://www.markdowntutorial.com/) from Markdown Tutorial. 

## Styling Text
Surround text with  
_one_ * or _ to make it *italic*  
__two__ * or _ to make it **bold**  
___three___ * or _ to make it ***italic and bold***, or you can __*mix*__ and **_match_** it  
~~two~~ ~ to ~~strikethrough~~ it  

``` markdown
Surround text with 
_one_ * or _ to make it *italic*
__two__ * or _ to make it **bold**
___three___ * or _ to make it ***italic and bold***, or you can __*mix*__ and **_match_** it
~~two~~ ~ to ~~strikethrough~~ it
```

---
## Headings
<!-- comment -->
# Heading is very easy
## Just add # in front of the text
### There are 6 levels of headings in total
#### The more \# you add 
##### The smaller the heading
###### Heading 6 is so small...
  
```
# Heading is very easy
## Just add # in front of the text
### There are 6 levels of headings in total
#### The more # 
##### The smaller the heading
###### Heading 6 is so small...
```

<!-- comment -->
## Paragraphs
It's also a good practice to keep articles clean and easy to read. We can do this by separating lines and adding sections.

To separating lines,  
we can add two spaces after each line.  
This is called a soft break.

```
To separating lines,  
we can add two spaces after each line.  
This is called a soft break.
```

You can also insert a hard break,

by adding empty line between lines.

```
You can also insert a hard break,

by adding empty line between lines.
```

To add a section (or horizontal line), use 3 - or * or _  
I usually use 

---
to make a horizontal line
```
To make a horizontal line / section, use 3 - or * or _  
I usually use 

---
to make a horizontal line
```

<!-- comment -->
## Links
The syntax for links are: `[text](link)`  
Surround **text** with [ ] to make it a link. Surround **link** with ( ).  

[This will bring you to Google.](https://www.google.com/)
```
[This will bring you to Google.](https://www.google.com/)
```
  
Another way to add links is using **reference link**.  

This is useful when you want to reference several text to the same [link][link-of-link], so you don't need to modify [one by one][link-of-link] when the [link][link-of-link] is updated or you want to change the [link][link-of-link]. 
All [links][link-of-link] in this paragraph are linked to the same link!

[link-of-link]: https://dictionary.cambridge.org/dictionary/english/link
```
Another way to add links is using **reference link**.  
This is useful when you want to reference several text to the same [link][link-of-link], so you don't need to modify [one by one][link-of-link] when the [link][link-of-link] is updated or you want to change the [link][link-of-link]. 
All [links][link-of-link] in this paragraph are linked to the same link!

[link-of-link]: https://dictionary.cambridge.org/dictionary/english/link
```


## Image
Embed image is similar to links.  
Add a **!** before [description of image (optional)](link to image).

![Black Cat](https://raw.githubusercontent.com/yinghei/ren-relaxing/master/static/img/black-cat.jpg)
```
![Black Cat](https://raw.githubusercontent.com/yinghei/ren-relaxing/master/static/img/black-cat.jpg)
```
  
Still remember ***reference links***? You can also do it with images!
  
## Lists
#### Ordered List
1. This is an ordered list
2. just type the number with a dot and a space
3. then it turns into a ordered list

#### Unordered List
* This is an unordered list
* type * or - followed by a space
* then it turns into a unordered list

#### More about list
1. list can be nested
	1. this is nested item
	2. another nested item
2. back to main level
	- nested item can change type 

- list can also contain italic and other markdown elements, such as
  - [links](https://www.google.com/)
  - ![images](https://yinghei.github.io/assets/img/avatar-icon.png)
  - `code snippets`
  - a soft  
    - break

```
#### Ordered List
1. This is an ordered list
2. just type the number with a dot and a space
3. then it turns into a ordered list

#### Unordered List
* This is an unordered list
* type * or - followed by a space
* then it turns into a unordered list

#### More about list
1. list can be nested
	1. this is nested item
	2. another nested item
2. back to main level
	- nested item can change type 

- list can also contain italic and other markdown elements, such as
  - [links](https://www.google.com/)
  - ![images](https://yinghei.github.io/assets/img/avatar-icon.png)
  - `code snippets`
  - a soft  
    - break
```


## Checkbox
- [x] this is a complete item 
- [ ] this is an incomplete item
```
- [x] this is a complete item 
- [ ] this is an incomplete item
```


<!-- comment -->
## Tables

| Headers | are shown | in bold |
| ------ |--- | --- |
| Add | new | row. |
| You | can | have |
| many | rows | ! |

```
| Headers | are shown | in bold |
| ------ |--- | --- |
| Add | new | row. |
| You | can | have |
| many | rows | ! |
```

## Code

There are quite a number of code chunks in this article.
Here's how you can make it:  

For inline code snippet, use one \`  to surround the text. `This become code snippet.`  
  
For code chunk, use three \` to surround the text.
```
text surrounded by ``` will become code
```

\`\`\`  
text surrounded by ``` will become code  
\`\`\`  
tips here: you can use \ to avoid ` turning into code snippet (in case you don't want to)  
   
  
This is also a code chunk, using three ~  
~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~
  
You can also specify the programming language. The code snippet will be generated with syntax highlighting:  
```python
def sum_2_numbers(a, b):
    return a + b

sum_2_numbers(2, 3)
```

\`\`\`python  
def sum_2_numbers(a, b):  
    return a + b  
  
sum_2_numbers(2, 3)  
\`\`\`

## Blockquotes
Blockquotes are block that stands out from others.
Block quotes can contain other elements, such as styling, links, or images.

> This is a **blockquote**  
> go to [next section](https://yinghei.github.io/ren-relaxing/basic-markdown/#comment)

Block quotes can contain other elements, such as styling, links, or images.

## Comment
When you want to jot notes for yourself, and don't want to let others see it, you can use comment!  
Comments are useful when you need to recall your logic / codes after a period of time.

<!-- This is comment which won't show up --> 
You can't see the comment.

```
<!-- This is comment which won't show up --> 
You can't see the comment.
```
