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

