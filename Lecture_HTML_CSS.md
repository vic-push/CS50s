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

There is a lot of more tags in HTML but they work in a similar way. They have tag and atributtes. 

## CSS
He starts with a basic way to add css to html, including style inside each tag. 
For example, to chage the style of `<h1>` we can do this:
`<h1 style="color: blue; text-align: center;"`
We can styles HTML element from a parent tag. For example if we write the style atributtes in the `body` tag instead of the `h1` tag they will apply to the hole section.
We have some more options to add style to our HTML page. One of them is adding an `style` tag inside the `<head>`. For example:
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





