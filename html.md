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

The very basic HTML structure is:

```html
<!DOCTYPE html>
<html lang="en">

  <head>
    <title>Basic HTML valid structure</title>
  </head>

  <body>
    <!-- Web Page Content -->
  <body>

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
We have a lot of **selectors** with some advance uses or universal selctor with `*`.
Remember, every browsers has his set of default values for styling.

You need to know that CSS Selectors (tag name selector, pseudo element selector, class selector, attribute selector, id selector, etc...) have different specificity in order to determine which style is applied to an element. The more specific a CSS style is, the higher point value it result. You can read more [here](https://dev.to/emmawedekind/css-specificity-1kca).
You also need to know the different between HTML tag selector and BODY tag selector. You can read more [here](https://css-tricks.com/html-vs-body-in-css/).
It's a best practice to use rem unit relative to the font-size of the html element, which is the document root.

The default size of font is 16px, so there's a convinient way to set font-size on bdoy at 62.5%, so you can adjsut the other font-size elements with a base size of 10px instead of 16px. So for others element you can use a size of 1.4em to have 14px or 1.4rem. Beware of using em instead try to use rem (root em) introduced by CSS3.
The em unit is relative to the font-size of the parent, which causes the compounding issue. The rem unit is relative to the root—or the html—element. That means that we can define a single font size on the html element and define all rem units to be a percentage of that.
So in this case we set 62.5% of font-size on the html tag element instead of body. We now have consistent and predictable sizing in all browsers, and resizable text in the current versions of all major browsers. [Read More](https://snook.ca/archives/html_and_css/font-size-with-rem)

# External Custom Style

So we can create our custom style and add it to our page. Create a file called 'style.css' and add to index.html with: 
```html
<head>
	<link rel="stylesheet" href="style.css">
</head>
```

```css
html {
  background-color: green;
}

body {
  background-color: yellow;
}
```

The body element doens't expand to cover the whole page.
The html element will use the backogrund color of body element, if its own is computed as transparent or none.
By default, body element has some margin from borders and the height is set based on its content.

```css
html {
  background-color: green;
  border: 1px solid red;
}

body {
  border: 1px solid blue;
}
```

as you can see body element is collapsed in one line and the html background color is bleeds past its border because the background color is propagated to the viewport, which is the canvas containing all the HTML elements.
You have a height of html because of the default body margin property.

The wildcard selector ( * ) selects ALL the elements in your document, including tags like html, body, p, h1, h2, h3, h4, h5, h6, form, input, button, textarea, select, option, legend, fieldset…I won’t list the entire reference, but you get the idea. Using the wildcard selector is bad practise in general.

I can reccomend to use a reset or normalize css in order to have gaininig control, predicatability and uniformity of your stylesheet.

So, let's start to write some style:

```css
html {
	font-size: 65.5%;
	box-sizing: border-box; /* Include padding and border in the element's total width and height */
}

body {
	font-family: 'Josefin Sans','Comic Sans MS', cursive, sans-serif;
	font-size: 1.6rem; /* =16px */
	margin: 0;
}

main, header, div, h1, h2, h3, h4, h5, h6, p, footer, section, a, ul {
	margin: 0;
	padding: 0;
}

a {
	text-decoration: none;
}

ul {
	list-style: none;
}

h1 {
	font-size: 2.4rem; /* =24px */
}

```

# Media Query

Don't forget to put in head tag:

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

or you media query maybe can't works!!!

# CSS Grid

Is a new feature of CSS specification, that allow us to position elements in two-way mode, instead of one-way mode of flexbox. In flexbox you can position your elements between a main axis and a cross axis. So, basically, you have a row and a column. We can configure flexbox two wrap more content in two rows or more rows (or columns), but is still one dimensional: a row of items or a column of items. With grid we have a real multi dimensional layout.

We can set a display to grid by using the value `grid` on display propery of a div, for example:

```
header {
	display: grid
}
```

same as using flexbox. I guess nothing change after this set, because the default behavior is to create, for each block element, a row. Same as flex.

# Tips

[Remove margin from li displayed inline](https://stackoverflow.com/questions/20805028/how-to-remove-the-default-margin-of-inline-li-elements)