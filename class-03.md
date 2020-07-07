# Reading 2

## Ducket HTML

### Chapter 3 "Lists"

In HTML we have 3 types of lists: ordereded lists, unordered lists and definitions list.

Ordered list uses the tag `<ol>` which puts every point or `<li>` in an ascending order like this :

<ol>
<li>First point</li>
<li>Second point</li>
<li>Third point</li>
</ol>

Unordered list uses the tag `<ul>` which puts every point or `<li>` in as a bullet point like this :

<ul>
<li>First point</li>
<li>Second point</li>
<li>Third point</li>
</ul>

Defined list uses the tag `<dl>` and usually contains pairs of the tag `<dt>` for the term and `<dd>` for the definition, and it puts the term with their definitions like this:

<dl>
<dt>First definition</dt>
<dd>This is the definition</dd>
<dt>Second definition</dt>
<dd>This is the definition</dd>
<dt>Third definition</dt>
<dd>This is the definition</dd>
</dl>

### Chapter 13 "Boxes"

Every element in HTML is contained within a box, which has many properties and can be modified. Some of these properties are mentioned below.

Boxes can have a specefic width and height, which means it won't take up the whole page, also boxes can consist of 3 layers, a border around the content, a padding around it, and a margin that seperates it from the other elements.

Boxes can also have a border that can have color and styles, and can also be hidden, another thing about boxes is that when you set a specefic size, you can make sure that the extra content overflows like you need it to, whether its hidden or scrolled upon.

## Ducket Javascript

### Chapter 4: “Decisions and Loops”

Continuing on the previous read, we go into switch statments, which are similar to if statments, but instead of using multiple, you just use switch with a paramter called switch value, and multiple cases that execute, and depending on the switch value, a case is executed, or the default case if no match is found.

Truthy and falsey values are important, since operators don't only check boolean values, they need to check values like that.

Loops
Loops are important as they can do the same task over and over as long as a certain condition is true, now you can use For While and Do...while, they all have a condition in common and the same format for (i=0;i<10;i++) {code}

