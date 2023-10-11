# David's Interview Study Guide

## Introduction

This is a fairly basic interview study guide. Why, you may ask? Well, it's because I don't know anything yet. I did complete a bootcamp hosted by University of California Riverside extension, but that is a broad spectrum intro to the world of development. I wish to learn more and ultimately get a job as a developer. Hopefully this might help you too. I will preface this study guide with the fact that this is strictly for #WebDevelopment

## HTML, CSS, JavaScript

### What is HTML, CSS, and JavaScript?

#### HTML

HTML stands for Hypertext Markup Language, it a markup language that adds the structure to a website. Almost all the actual information on a webpage is represented in HTML tags. These Tags are what break up the content into different sections. It is generally a good practice to use semantic tags.

_What are semantic tags you may ask?_

Semantic tags are tags that clearly let the browser and the developer know what will be contained in that tag. Examples of some semantic tags are `<nav>`, `<main>` or `<article>`.
Some examples of some non-semantic tags are the infamous `<div>` and `<span> `

Below we have two examples the one on top is the non-sematic HTML tag set up, The one below is the best practice semantic version

##### Non-Semantic HTML

```
	<html>
			<head>
					<title>Non-Semantic Example</title>
			</head>
			<body>
				<div>
						<ul>
							<li><a href="Home.html"> Home </a></li>
							<li><a href="About.html"> About </a></li>
						</ul>
				</div>
				<div>
						<h1>This is Non-Sematic Tags</h1>
						<p>This is a paragraph</p>
				</div>
			</body>
	</html>
```

##### Semantic HTML

```
	<html>
			<head>
					<title>Semantic Example</title>
			</head>
			<body>
				<nav>
						<ul>
							<li><a href="Home.html"> Home </a></li>
							<li><a href="About.html"> About </a></li>
						</ul>
				</nav>
				<main>
						<h1>This is Non-Sematic Tags</h1>
						<p>This is a paragraph</p>
				</main>
			</body>
	</html>
```

#### CSS

CSS stands for cascading style sheets. CSS is what gives most websites its appearance. CSS is used to style the HTML elements. CSS is also used to make a website responsive. Responsiveness is an extremely important part of web development as most users access websites through a mobile device.There is a common design principle to make all website design mobile first. This means that the website is designed for mobile first and then expanded to fit a desktop screen. This is done because it is easier to expand a design than to shrink it. Another important part of css is that if you apply a style to one element it will flow down to all the child elements unless otherwise specified, this is called cascading.

CSS operates with selectors, these can be html tag or can select a specific class or id. CSS can also be used to select a specific element within another element. This is called a child selector. CSS can also be used to select a specific element that is next to another element. This is called an adjacent selector.

There are some common CSS properties that are used to style a website. These are:

**margin** - This is the space outside of an element
**padding** - This is the space inside of an element
**border** - This is the border of an element
**background** - This is the background of an element
**color** - This is the color of the text
**font-size** - This is the size of the text
**font-family** - This is the font of the text
**font-weight** - This is the weight of the text
**text-align** - This is the alignment of the text
**display** - This is how the element is displayed

It is extremely important to understand the concepts behind flexbox and grid. These are the two most common ways to style a website. **Flexbox** is used to style a website in a one dimensional way. **Grid** is used to style a website in a two dimensional way. I can not really describe these in an accurate way because I still do not get it. I just use trail and error to get the desired result.

#### Some other CSS things to know are:

**CSS Variables** - These are variables that can be used in css

```
/* this is how you declare a css variable */

	:root {
		--main-color: #000000;
	}

/* this is how you use a css variable */

		.main {
			color: var(--main-color);
		}
```

**Media Queries** - These are used to make a website responsive

```
/* this is how you declare a media query */

	@media screen and (max-width: 600px) {
		body {
			background-color: lightblue;
		}
	}
/* this will make the background color light blue when the screen is less than 600px */
```

**Animations**- These are used to animate elements on a website

```
/* this is how you declare an animation */
	@keyframes example {
		from {background-color: red;}
		to {background-color: yellow;}
	}
```

As stated above CSS is mostly trail and error so I would recommend just playing around with it to get a feel for it. If you are getting some funky results I would recommend using the inspect tool in your browser to see what is going on, you can also add and outline to all elements on your page to see how they are interacting with each other.
This is done by adding the following code to your css file.

```
	* {
		outline: 1px solid red;
	}
```

#### JavaScript

Javascript is a programming language that is used to add functionality to a website. Javascript is used to make a website interactive, dynamic, and make a website responsive.
