# Reading 6

## External Reading

### Problem Domain

The problem domain is like a jigsaw puzzle, the clearer it is the easier it is to code. Now in order to make it easier, one should understand it more, and then after deepnening your understanding you can make the domain easier, which eases the coding.


## Ducket JavaScript

### Chapter 3 "Object laterals"

In an objects, variables become proepries, and functions become methods.

Properties names are called keys, and they need to be unique.

To create objects one uses literal notation which is something that uses colon to speerate between names/keys and values, and commas to seperate between each property, also you can acess the obects using a dot like class in CSS, or using `["property"]`:

```
var someObject : {
    property1:value,
    property2:value,
    property3:value,
    someFunction: functoin {
        return this.property1 - someObject.property2 + someObject["property3];
    }

}
```

### Chapter 5 "DOM"

DOM stands for Document object model which is a seperate set of rules that specifies how the javascript and the html page should interact. The browser saves a model of the HTML page in its memory, and then the DOM shows how to interact, what it can ask and how to change.

API stands for Application programming interface, which is how programs interact with each other, what and how can they change and ask for things. 

**DOM tree** is a way to show the elements and components of the HTML page, as you can see below in the attatched picture, this is how a DOM tree looks like, and it uses the same terms as parent, child, grandchild.

![DOM Tree](https://www.tutorialrepublic.com/lib/images/html-dom-illustration.png)