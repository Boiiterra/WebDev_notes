# Learning HTML
This contains some useful info about HTML. \
Soon will organize it.

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
Has attribute `target`. If you set target to `_blank` link will open in new tab/window, if target is set to `_self` which is default then link will open in current tab.

<a href="https://google.com">'Google' with no extra attributes</a><br>
<a href="https://google.com" target=_blank>'Google' with blank</a><br>
<a href="https://google.com" target=_self>'Google' with self</a>


Code:
```html
<a href="https://google.com">'Google' with no extra attributes</a><br>
<a href="https://google.com" target=_blank>'Google' with blank</a><br>
<a href="https://google.com" target=_self>'Google' with self</a>
```
