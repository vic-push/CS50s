The course starts with HTML and CSS, after that we are going to introduce Git to use control version. After Python (Django), SQL..., JavaScript. Next we will move to Testing and CI/CD and finally with Scalability and Security.

# HTML & CSS
## DOM
Basically the DOM is just a way to organize tags so that some are inside others.

## List
HTML has two types of list, ordered list (```<ol></ol>```) and unordered list (```<ul></ul>```). 
To use the ordered or unordered list you can set the items of the list with the tag ```<li></li>```

## Media 
### Images
The tag to use images inside the html file is: <img></img> but has a couple of attributes that are mandatory. Below is an example of a full line of a image with the attributes necesaries to be correct and work it
  ```<img src="cat.jpg" alt="Cat">```
The images tag does not have ending tag. Besides the attributes mentionated above, the image tag has some others like:
- Width: to adjust the width with pixel
- height: to adjust the height with pixel
In adittion, the src of the image could be an url where the image is.

### Link
```<a href> ``` is the tag used to link a url to a word that will be writting inside of the open and closed a tag. Instead of external url, with this tag you can link yours owns html pages just writting.

### Tables
To create a table we need to start by using the <table></table> tag that represents the entirety of the table. Inside the table, we have some different parts: heading, body...
- The tag <thead></thead> is used to build the heading of the table
  - The tag <th> is inside of <thead> and used to create each "column" of the table heading.
- The tag <tbody> contains the main information of the table.
- Inside the <tbody> we have one tag <tr> for each row who is going to contains the information of each cell thanks to the tag <td></td>

## Form
To start with a form you need to begin with a form element (tag) ```<form></form>
Inside these tags you should add each field of the form with the correct tag.
Some of them are:
### input tag
An input tag ```<input>``` is used when you want the user insert text in a field. This tag has some important attributes:
- type (text, number, submit...)
- placeholder --> the words or sentence written in the field
- name --> A name for this input specifically. This attribute is quite important bearing in mind could be a lot of tag input in a single form.
### datalist w/ option
The tag ```<datalist>```is used to make a selectable list in a form. Datalist is filled with options, that options are named with the tag ```<option>```
Use datalist instead of select is the best option because in Select you only can select one option of the list but in datalist you have the posibility to write and search above the options.
But if you want to use the datalist you need to make an input field to connect with. In the next lines displays an example of how do it.
```
  <input name="browser" list="browsers" placeholder="browser">
    <datalist id="browsers">
        <option value="Chrome">
        <option value="Firefox">
        <option value="Safari">
        <option value="Opera">
        <option value="Edge">
    </datalist>
```

There are many more tags in HTML but they work in a similar way. Each tag can have attributes. 

## CSS
He starts with a basic way to add css to html, including style inside each tag. 
For example, to change the style of `<h1>` we can do this:
`<h1 style="color: blue; text-align: center;"`
We can style HTML elements from a parent tag. For example, if we write the style attributes in the `body` tag instead of the `h1` tag they will apply to the whole section.
We have some more options to add style to our HTML page. One of them is adding a `<style>` tag inside the `<head>`. For example:
```
<head>
  <title>Hello!</title>
  <style>
    h1 {
        color: blue;
        text-align: center;
    }
  </style>
</head>
```

The other option -and in my opinion the best- is to create a new file (.css) where we put all the style and link it with the HTML page.
To link the css page to the HTML page we use `<link rel="stylesheet" href="styles.css">`

### Some important attributes in CSS
- background-color --> used to change color of the background
- width --> to chage the widht (ancho) of a div for example. Normally in pixel measure
- height --> to chage the height (alto) of a div for example. Normally in pixel measure
- padding --> to create padding (espacio) inside the element. For example, if we have a div with text inside, this style attribute will separe the text from the border of the div. Normally in pixel measure
- margin --> to create space outside of the element. For example, if we have a div, this style attribute will add a space between the border of the browser page and the div element.
- font-family --> to chang the font of the text. We can specify multiple fonts just in case some devices can not support the font. Is important to add some backup font just in case.
- font-size --> this attribute is used to specify the size of the text. Normally is written in pixel. For example `font-size: 28px;`
- font-weight --> this attribute is used, normally, to make the text into a bold way.
- border --> this attribute is used to make a border around section. The most used way is in div section. Inside this attribute you can specify differents settings of the border, for example, solid if you want to have a continuous line, 3px for the width or black for the color.
- border-collapse:collapse --> this attribute is used to collapse the border of the cells and the table. 

## ID's
If you want to change the style of some elements that share the same tag you can give an ID to an specific tag. In the next example we can see how this work:
```
<style>
  #title_one {
    color: blue;
  }
  #title_two {
  color: red;
  }
</style>
<h1 id="title_one"> Heading 1 </h1>
<h1 id="title_two"> Heading 2 </h1>
<h1> Heading 3 </h1>
```
We can see that the first and second `<h1>`tag have an attribute called id. Thanks to that we can modified through the style sheet those tags using the special character #.

Another similar attribute is the class. The class are used when we want to modify some elements in the same way. We should not use the same id for different tags because it could cause some troubles. For this reason we should use the class. We can modify a class in the style sheet using a dot (.) before name it. For example:
```
<style>
  .baz {
    color: blue;
    
  }
</style>
<h1 class="baz"> Heading 1 </h1>
<h1 class="baz"> Heading 2 </h1>
<h1> Heading 3 </h1>
```
## Theoretical concept of specificity
We are seeing how many options are possible to change the style of elements of a HTML page thanks to CSS. But this have some difficulties of management and that are the specificity. What changes are goingo to apply if we modify the style with the id, the class and inline. To solve this problem, we can follow the next list of priorities:
1. inline
2. id
3. class
4. type

At first is confusing but in reality is very useful. For example, imagine we want to have all the `<h1>`with the same font but we want that one particularly has a specific color. We can do a class for all of them and in addition, put an id in the specific `<h1>`. The result will be all `<h1>` with the same style and that different one will have only the little changes we did with the id.





