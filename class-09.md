# Reading 8

## Ducket HTML & CSS

### Chapter 7 "Forms"

Forms are widely used for their ability to collect information from users, which is one of the first ways we learn on how to interact with the user. Now it could have multiple ways, they can be text forms that take in one line, password or muli lines. They could also be forms that have radio buttons, checkboxes or dropdown list. 

![HTML form](https://mobile.htmlgoodies.com/imagesvr_ce/1902/HTML%20Form.PNG)

For that to happen one uses the tag `<form>` and inside it one uses two attributes, the method which is between get and post, and the action which is the url of the page that process the information inside the form. As for the methods each method has its own attribute for example ```<input type="search">``` and many others.


### Chapter 14 "Lists, Tables & Forms"

When dealing with lists, CSS can change the style of lists, whether its ordered or unordered. Each of them has their own styles, where you can specify the style of the marker, and if its inside or ouside the box which is about identiation.

As for tables, you would need to style the headers, data, empty cells, borders, backgrounds and colors. This can be done within CSS ofcourse, and it changes the looks and makes it easier to know which data is which in the table.

Same thing for forms, where one can change the icons the fieldsets and the legend, and the color size font and size of it all.

![table](https://i.stack.imgur.com/vslIt.png)


## Ducket JavaScript

### Chapter 6 "Events"

Whenever something happens in the browser its called an event, and these events help us interact with the browser, by **triggering** functions when these events are **fired/raised**. Now there are many events like: onload, onclick, onblur ... etc. And to interact with these event there are three ways:

1-HTML handler which is not recommended since its a good practice to seperate HTML and javascript.

2-DOM handlers which are useable but they can't trigger more than one function at the same time.

3-DOM Level 2 event listners, which can trigger more than one function with parameters.

![Events](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/Ways-of-Using-JavaScript-Events.png)

**Flow** of events matters, since if its a bubble then it starts from the most specific then moves to the least, but if its an event caputring then it startes from the least specefic/most general to the most specefic.