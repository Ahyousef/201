# Reading 2

## Ducket HTML

### Chapter 2 "Text"

**Visual editors** like visual studio code, usually have two sides, one for the code display which shows the code as its being written, and the other visual disaply, that previews the final look.

#### Structural markup

**Headings** tags make the text bolder and bigger, and it has six levels, starts from the largest `<h1>` and ends with the smallest `<h2>`.

**Paragraph** tag contains one or more sentences of text, and each tag puts the text on a new line with some space in-between. To create the paragraph, use tag `<p>`

**Bold and *italic*** tags can make the text **bold** by using `<b>` tag. and make make the text *italic* through the use of `<i>` tag.

**Superscript and subscript** tags can be useful when wanting to put things like 4<sup>th</sup> or 2<sub>nd</sub>. To use them wrap the intended text in the tags `<sup> or <sub>` depending on the usage

**White space** in html is collapsing, meaning html will treat all white space as one, so in order to make breaks one needs to use `<br>` tag. As for horizental rules use `<hr>` tag.

#### Semantic markup

![semantic](https://enlightsolution.com/wp-content/uploads/2019/06/pic-1-300x187.jpg)

**Strong and emphasis** The use of `<strong> and <em>` shows that the content is important, and for emphasis it shows content in italic by default.

**Quotation** When wanting to quote short quotes, one uses the element `<q>` but for longer blocky quotes one uses `<blackquote>` element.

**Acronyms and abbreviation** Use the element `<abbr>`.

**Citations, definitions and author details** To cite something use the element `<cite>` and for definition use `<dfn>`, and finally for details of the author use `<address>`.

**Content edit** Use `<ins>` for inserted content, `<del>` deleted content, and `<s>` for content that is not accurate anymore.

### Chapter 10 "CSS"

# CSS

Since HTML is the skeleton of the webpage body, CSS can be considered as the skin of that body. CSS is used to present and make the webpage look better and nicer, this includes colors, backgrounds, fonts, allinging and many more. CSS stands for Cascading Style Sheet, and it normally exists as a seperate file ith a .css extension, but can also exist within the HTML file but that is a bad practice.

## Format

In CSS you can create a class like `.blue` or target an element in the whole page `p ` or elements within a certain parent `nav p` and you can use commands to change many things like border, padding, margin and color

### Colors

Many ways exist in CSS to specify the color, you can use hixdecimal #fffff, or Red Green Blue (RGB), Or HSL stands for hue, saturation, and lightness, and finally some colors exist as their names like red and orange and others.

## Ducket Javascript

### Chapter 2 "Basic JavaScript Instructions"

**Script** can be seen as instructions for the computer on what to do, and it is made out of seperate lines, each line is called a statment.

**Comments** can be left for clarification or to disable certain lines out of the code, this can be done using // for one line, and /* */ for block comment.

**Variables** are like containers that can contain different values, and can be called upon in the script.

**Data types** are mainly 3, string for text, number for numerical values and boolean for true and false.

**Arrays** are considered as a list that contains more than one value, like a shopping list for example.

**Operators**

Operator | Name | Usage
-------- | ---- | -----
+ | Addition| Adds two values
- | Subtraction | Subtracts two values
* | Multiplication | Multiplies
/ | Division | Divides two numbers
++ | Increment | Adds to the existing
-- | Decrement | Subtracts from the existing
% | Modulus | Shows the remidner

## Chapter 4 "Decisions and loops"

Just like humans, the script needs to make decisions, think of it as when you need to go out, if its raining you take an umbrella, if its not you don't. 

The computer does a similar thing, by evaluating and executing statments, for example :
<br>
` if (age >= 18) {enter = true}`

![flowchart](https://www.syncfusion.com/products/essential-js2/control/images/diagram/flowchart.png)