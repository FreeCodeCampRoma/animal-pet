# Webpage

A website is a collection of webpage that are often related to each other.
A webpage consists of three main technologies: HTML, CSS and JavaScript. These are the computer languages understandedable by a browser.
HTML stands for HyperText Markup Language, a language where is grammar is a set of markup called tag name.
What I do find helpful is explaining that HTML is a coding language for displaying information.
HTML structures the content of a web page into a bunch of boxes.
Inside each box we can have a combination of boxes, text, images, and others.
By default, boxes size are as high and as wide as their contents or we can set a default size for both width and height properties.
The whole HTML box consists of the opening tag, closing tag and contents, and this is all called an HTML Element.
The opening tag is made up by "<" (also called chevron, angle brackets) + tag name + ">".
The closing tag is made up by "<" + "/" (also know as "forward slash") + ">".
Example:

```html
<div>Hello HTML</div>
```

The contents can be others HTML Elements, Text or can be empty.
The default way to display HTML Elements in the documents is from the top to bottom.
Is it all? No, we have he ability to adds attribute inside the opening tag for add behaviours, change layout with style or add some unique identifier.
An attribute is made up of a name, an equal simbol and a value. It is a key-value pair where the value is wrapped in a single or double quotes.
Each HTML Elements can have his sets of attribute differents from other HTML Elements such as the HTML Element for displaying an image, it has attribute for identify the file of the picture, or the HTML Element for URL navigation has an attribute contains the web address.
Some of these elements are semantic meaning for improve search engine ranking and manutenability of the webpage itself.

When we load a webpage, we can inspect it with Developer Tools inside Goolge Chrome, and we can change contents and tags and see which properties are applied and we can change it in real-time.
[Download it](https://www.google.com/intl/en/chrome/)

# Github

[Download it](https://desktop.github.com/)
You can use github desktop to publish and share your code. After installed it, you can choose a local folder as a repository, on your computer and set it as your folder project (you don't need to create it, you can choose Desktop destiantion then software will create a sub folder with the name of the project you have choosen).
A repository (called repo) is a box where we can store our files and monitor all the changes we will do to our files.
When we do some bunch of changes on our code, we can check for "changes" tab on our desktop github application.
If we see a green plus icon near a file it's a new file, when we see a yellow point it's a changed file.
To make our changes applied we need to commit it. After a commit we can check "History" tab. 

Register for a free account on github.com, in this manner we can push our code on github. It is also use as a backup tool.

# Editor

[Download it](https://code.visualstudio.com/)
There are a bunch of good editors you can use on Win, Mac and Linux such as Sublime, Atom, Webstorm and Visual Studio Code. I can suggest the last two editors, the first one is a complete IDE you can use for non commercial project, the second is an open source editor from Microsoft, it is the most used by developers.

# First web page

We can write our first page by creating a file called index.html and write some HTML Elements:

```html
<h1>My Pet friends</h1>
<p>Hey, welcome to my page about my <b>pet friends</b>. They <b>improve and enjoy</b> my life and make my home <b>coolest</b>.</p>
<img src="images/cat.png">
```

As you can see some opening tags doesn't need a closing tag such as Image HTML Element or Line Break HTML Element "<br>". They are self closing HTML Element and sometimes we add attribute to enrich the behaviour and content.
When you inspect this little page, you can see that our browser will ad some HTML tags such as head, body and html. This tag are not mandatory but it's a best practice to add it in our code.
The head tag element contains all the metadata of our webpage and its content is not visible. The title is mandatory.
The body element is where we put all of our visible content.
It's important to pay attention to indentation of our source code for readability and understand which boxes contains other boxes or elements.
Finally we need DOCTYPE tag, that identify our document:

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<title>Animal Pet</title>
</head>
<body>
	<h1>My Pet friends</h1>
	<p>Hey, welcome to my page about my <b>pet friends</b>. They <b>improve and enjoy</b> my life and make my home <b>coolest</b>.</p>
	<img src="images/cat.png">
</body>
</html>
```

When we had to write a more complex website, it's useful to use something like a wireframe software or paper and pen and do something like a sketch of the elements of the webpage ![Wireframe](https://d33wubrfki0l68.cloudfront.net/dbb80f2f6a5dafa25f702ad00bc429057fb59cec/52716/en/blog/uploads/versions/samuel-student-wireframe---x----972-715x---.png)

# Style

We can add our own style to HTML elements such as "background-color", "width", "height", thank to CSS - Cascade Style Sheet. He makes HTML looks better by overriding default style provided by the Browser.
A CSS consist in a set of key-pair value, with the name of the property, a semicolon and the value. Sometimes the value need a unit measure like px, em, rem o hexadecimal value. Tehre are tons of properties we can change to control how an element looks and feels.
We can apply our custom CSS rule in three ways (in order of precedence if I have the same rule with different value - css specificity): inline (directly to the element), embedded (inside a couple of tag style within head tag) and external file(the preferred way) using link tag element.

```html
<head>
	<title>Animal Pet</title>
	<style>
		h3 {
			font-weight: 300;
			color: teal;
		}
	</style>
	<link rel="stylesheet" href="style.css">
</head>
<body>
	<h1 style="font-family:Courier New, sans-serif; font-size:28px; color:#FF5732;">Hello CSS</h1>
	<h2 style="font-size:18px; color:violet;">We are learning!</h2>
</body>
```

We can add styles by selecting a specific element such as by tagname or by identification attribute, or by selection all certain kind of element such as all h1 or p element or by selecting elements in a certain position such as all the descend of a specific element or class of elements, or selecting elements with some attribute and value. 
We have a lot of **selectors** with some advance uses or universal selctor with '*'.
Remember, every browsers has his set of default values for styling.
