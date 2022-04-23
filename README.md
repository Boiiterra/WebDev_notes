# Learning HTML
This contains some useful info about HTML. \
Soon will organize it. \
If you struggle to understand what the hell is here well this is my notes for HTML.
You can fork it and change it if you like.

## Main structure

For HTML5:

```html
<!DOCTYPE html>

<html>

<head>
<!--User does'nt really see whats here-->    
</head>
<body>
<!--What user will see-->
</body>

</html>

```

## Websites title

To change websites title use:
```html
<title>Title</title>
```

## Headers

You can add up to six different headers to your website:
Example:
<h1>Header 1</h1>
<h2>Header 2</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>

Code:

```html
<h1>Header 1</h1>
<h2>Header 1</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
```

## Paragraph

Is an element that has blank line before and after it:

<p>Paragraph example</p>

Code:

```html
<p>Paragraph example</p>
```

## Line breaker
This element doesn't require closing tag. Adds line break 

<br>

code:

```html
<br>
```

## Horizontal rule
This element doesn't require closing tag. Devides page by sections 

<hr>

Code:
```html
<hr>
```
## Hyperlinks
Element of the page surrounded by `a` tags that refers to something
Has attribute `target`. If you set target to `_blank` link will open in new tab/window, if target is set to `_self` which is default then link will open in current tab. Also there is useful attribute `title` which displays tip box when hover over link. Links can also be used to redirect user to another page. To do so you need to insert path to necessary html file in main one into `href` attribute.
To begin sending email process you need to insert `mailto:email@email.example` into `href` attribute

<a href="https://google.com">'Google' with no extra attributes</a><br>
<a href="https://google.com" target=_blank>'Google' with blank</a><br>
<a href="https://google.com" target=_self>'Google' with self</a><br>
<a href="https://google.com" title="Title">'Google' with title</a>


Code:
```html
<a href="https://google.com">'Google' with no extra attributes</a><br>
<a href="https://google.com" target=_blank>'Google' with blank</a><br>
<a href="https://google.com" target=_self>'Google' with self</a><br>
<a href="https://google.com" title="Title">'Google' with title</a>
```

## Images
To display images you need to use image element `img` which is self closing tag
and change it's source attribute. Also you can change size of the image. To do so you need to use `width` and `height` attributes (This attributes are in **PIXELS**). In order to scale an image you can change only one attribute. To add alternative text to the image you need to use `alt` attribute. To add a pop up text box use `title` attribute. If you want to add hyperlink to the image simply surround it with `a` tags and add link to `href` attribute of `a` tag. 

<img src="images/example.jpg" alt="This is an example image"><br>
<a href="https://commons.wikimedia.org/wiki/Example_images"><img src="images/example.jpg" alt="image" title="Link to the image source"></a><br>
<img src="images/example.jpg" width=280, height=110 title="Is it wide?">

Code:
```html
<img src="images/example.jpg" alt="This is an example image"><br>
<a href="https://commons.wikimedia.org/wiki/Example_images"><img src="images/example.jpg" alt="image" title="Link to the image source"></a><br>
<img src="images/example.jpg" width=180, height=110>
```