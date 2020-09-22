# INTRO-CSS

If HTML is marking and structuring text using elements. CSS is styling the elements. You use CSS to add color, add space make the font a little bigger, hiding and showing them, add a round border, make the border thinner / thicker etc. Oh and CSS stands for **C**ascading **S**tyle **S**heets in case your were wondering.

Let me just show you. Here is some HTML markup:

    <!DOCTYPE html>
    <html>
	    <head>
	    	<title>HTML example</title>
	    </head>
	    <body>
		    <h1>My First CSS Example</h1>
		    <p>This is a paragraph.</p>
	    </body>
    </html>

It looks like this when rendered (in browser)

![rendering of the html markup above it](https://raw.githubusercontent.com/Team-FCB/Assets/master/html_simple_markup.png)

Let's add some CSS

    <!DOCTYPE html>
    <html>
	    <head>
		    <title>HTML example</title>
		    <style>
			    body {
			      background-color: purple;
			    }
			    h1 {
			      color: white;
			      text-align: center;
			    }
			    p {
			      color: white;
			      font-family: verdana;
			      font-size: 20px;
			    }
		    </style>
	    </head>
	    <body>
		    <h1>My First CSS Example</h1>
		    <p>This is a paragraph.</p>
	    </body>
    </html>

And this is how it looks now:

![HTML rendering with CSS](https://raw.githubusercontent.com/Team-FCB/Assets/master/html_simple_render.png)

We changed the background, text colors and also centered the header (h1) element.

## Simple CSS Breakdown

![Simple CSS Selector example](https://raw.githubusercontent.com/Team-FCB/Assets/master/css_selector.gif)

Credit: W3Schools

So with the standard spacing the above example would look something like this:

    h1 {
		color: blue;
		font-size: 12px;
    }

## Selectors

You cannot style an element unless you select it first unless you of course do in-element styling but more on that later. There are multiple ways to select an element for styling purposes.

-   Simple selectors (select elements based on name, id, class)
-   [Combinator selectors](https://www.w3schools.com/css/css_combinators.asp)  (select elements based on a specific relationship between them)
-   [Pseudo-class selectors](https://www.w3schools.com/css/css_pseudo_classes.asp)  (select elements based on a certain state)
-   [Pseudo-elements selectors](https://www.w3schools.com/css/css_pseudo_elements.asp)  (select and style a part of an element)
-   [Attribute selectors](https://www.w3schools.com/css/css_attribute_selectors.asp)  (select elements based on an attribute or attribute value)

Credit: W3Schools

We are just going to focus on simple select for now.
There are three ways we can select an element: id, class and name.

## Simple Selector

Here are three ways you can select the element below.

    <div class="container" id="main-container"></div>

### Simple Select by name

Very generic. Will apply to **ALL** divs.

    div {
    	color: blue;
    }

### Simple Select by id

Very unique. Will select only **ONE** element.

    #main-container {
    	color: blue;
    }

### Simple Select by class

This selector in between specific and broad. You can select a set of elements that share the same class name. Notice the period right before the selector class name!

    .main-container {
    	color: blue;
    }

`*` means select every element!

    * {
    	 color: blue;
     }

## Group Selector

What if you wanted to select and style multiple elements? Simple, seperate them with a comma. So something like this:

    p, .container, #container {
    	color: blue;
    }

## Continue on W3 Schools

Please finish reading up on CSS on W3 schools CSS tutorial site:

https://www.w3schools.com/css/
