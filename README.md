<details>
<summary><b>Navigation</b></summary>

- [HTML notes](#html-notes)
  - [Main structure](#main-structure)
  - [Websites title](#websites-title)
  - [Headers](#headers)
  - [Paragraph](#paragraph)
  - [Line breaker](#line-breaker)
  - [Horizontal rule](#horizontal-rule)
  - [Hyperlinks](#hyperlinks)
  - [Image](#image)
  - [Audio](#audio)
  - [Video](#video)
  - [Text formatting tags](#text-formatting-tags)
  - [Lists](#lists)
    - [Unordered list](#unordered-list)
    - [Ordered list](#ordered-list)
    - [Description list](#description-list)
  - [Tables](#tables)
  - [Colorful page](#colorful-page)
  - [Span and div](#span-and-div)

</details>
<hr>
<a href="https://terraboii.github.io/HTML_notes/"><p><b>Link to the Webpage</b></p></a>
<hr>

<br>

# HTML notes
This contains some useful info about HTML. Some examples are not supported here so you can view [Website]("https://google.com" "Link to the website") \
If you struggle to understand what is written here well this is my notes for HTML.
You can fork it and change it if you like.

<br>

## Main structure

For HTML5:

<br>

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

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Websites title

To change websites title use:

<br>

```html
<title>Title</title>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Headers

You can add up to six different headers to your website:
Example:

<br>
<h1>Header 1</h1>
<h2>Header 2</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
<br>

Code:

<br>

```html
<h1>Header 1</h1>
<h2>Header 1</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Paragraph

Is an element that has blank line before and after it:

<br>
<p>Paragraph example</p>
<br>

Code:

<br>

```html
<p>Paragraph example</p>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Line breaker
This element doesn't require closing tag. Adds line break 

<br>
<p>Line 1</p>
<br>
<p>Line 2</p>

code:

<br>

```html
<p>Line 1</p>
<br>
<p>Line 2</p>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Horizontal rule
This element doesn't require closing tag. Devides page by sections 

<br>
<hr>
<br>

Code:

<br>

```html
<hr>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Hyperlinks
Element of the page surrounded by `a` tags that refers to something
Has attribute `target`. If you set target to `_blank` link will open in new tab/window, if target is set to `_self` which is default then link will open in current tab. Also there is useful attribute `title` which displays tip box when hover over link. Links can also be used to redirect user to another page. To do so you need to insert path to necessary html file in main one into `href` attribute.
To begin sending email process you need to insert `mailto:email@email.example` into `href` attribute

<br>

<a href="https://google.com">'Google' with no extra attributes</a><br>
<a href="https://google.com" target=_blank>'Google' with blank</a><br>
<a href="https://google.com" target=_self>'Google' with self</a><br>
<a href="https://google.com" title="Title">'Google' with title</a>

<br>

Code:

<br>

```html
<a href="https://google.com">'Google' with no extra attributes</a><br>
<a href="https://google.com" target=_blank>'Google' with blank</a><br>
<a href="https://google.com" target=_self>'Google' with self</a><br>
<a href="https://google.com" title="Title">'Google' with title</a>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Image
To display images you need to use image element `img` which is self closing tag
and change it's source attribute. Also you can change size of the image. To do so you need to use `width` and `height` attributes (This attributes are in **PIXELS**). In order to scale an image you can change only one attribute. To add alternative text to the image you need to use `alt` attribute. To add a pop up text box use `title` attribute. If you want to add hyperlink to the image simply surround it with `a` tags and add link to `href` attribute of `a` tag. 

<br>

<img src="images/example.jpg" alt="This is an example image"><br>
<a href="https://commons.wikimedia.org/wiki/Example_images"><img src="images/example.jpg" alt="image" title="Link to the image source" width=180></a><br>
<img src="images/example.jpg" width=280, height=110 title="Is it wide?">

<br>

Code:

<br>

```html
<img src="images/example.jpg" alt="This is an example image"><br>
<a href="https://commons.wikimedia.org/wiki/Example_images"><img src="images/example.jpg" alt="image" title="Link to the image source"></a><br>
<img src="images/example.jpg" width=180, height=110>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Audio
To add audio files to your page use `audio` element (It has closing tag between which you can list sources in case one is not supported by browser).
You can add controls to an audio with `controls` attribute. You can make it auto play with `autoplay` attribute as well as muted (`muted`) and looped (`loop`)

Code:

<br>

```html
<audio controls src="/sample3.mp3"></audio>
<audio controls src="/sample3.mp3" autoplay muted loop></audio>
<audio controls>
    <source src="/sample3.mp3">
    <source src="/sample3.wav">
    This browser does not support HTML5
</audio>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Video
MP4, Ogg and WebM maybe some more. is quite similar to [Audio](#audio) and [Image](#image). Has closing tag which functions as [Audio's](#audio)

Code:

<br>

```html
<video controls autoplay muted loop src="sample_960x400_ocean_with_audio.mp4" width="400"><br>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Text formatting tags
Some of them.

<br>

<p>This is normal text</p>
<p>This is <b>bold</b> text</p>
<p>This is <i>italic</i> text</p>
<p>This is <big>big</big> text</p>
<p>This is <small>small</small> text</p>
<p>This is <sub>subscript</sub> text</p>
<p>This is <sup>superscript</sup> text</p>
<p>This is <ins>inserted</ins> text</p>
<p>This is <del>deleted</del> text</p>
<p>This is <mark>marked</mark> text</p>
<br>
Code:

<br>

```html
<p>This is normal text</p>
<p>This is <b>bold</b> text</p>
<p>This is <i>italic</i> text</p>
<p>This is <big>big</big> text</p>
<p>This is <small>small</small> text</p>
<p>This is <sub>subscript</sub> text</p>
<p>This is <sup>superscript</sup> text</p>
<p>This is <ins>inserted</ins> text</p>
<p>This is <del>deleted</del> text</p>
<p>This is <mark>marked</mark> text</p>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Lists 
<br>

### Unordered list
<br>
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3
        <ul>
            <li>Subitem 1</li>
        </ul>
    </li>
</ul>
<br>

### Ordered list
<br>
<ol type="A">
    <li>First
        <ol>
            <li>Subitem 1</li>
        </ol>
    </li>
    <li>Second</li>
    <li>Third</li>
</ol>
<br>

### Description list
<br>
<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
<br>

Code:

<br>

```html
<h3>Unordered list</h3>

<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3
        <ul>
            <li>Subitem 1</li>
        </ul>
    </li>
</ul>

<h3>Ordered list</h3>

<ol type="A">
    <li>First
        <ol>
            <li>Subitem 1</li>
        </ol>
    </li>
    <li>Second</li>
    <li>Third</li>
</ol>

<h3>Description list</h3>

<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
```


<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Tables
Is an arrangement of information or data usually represented in rows and columns.

<br>
<details>
<summary title="Some other elements can also have some same attributes">Attributes</summary>
    <ol>
        <li><b>bgcolor</b> - background color</li>
        <li><b>align</b> - aligns text</li>
        <li><b>width</b> - width of an element</li>
        <li><b>height</b> - height of an element</li>
    </ol>
</details>
<br>
<br>
<p>Basic one:</p>

<table>
    <tr>
        <th>Table Header 1</th>
        <th>Table Header 2</th>
    </tr>
    <tr>
        <td>Table Data 1</td>
        <td>Table Data 2</td>
    </tr>
</table>
<br>
<p>Modified one:</p>
<table bgcolor="black">
    <tr bgcolor="green" align="center" width="200">
        <th width="100">Table Header 1</th>
        <th width="100">Table Header 2</th>
    </tr>
    <tr bgcolor="lightgreen" align="center">
        <td height="50">Table Data 1</td>
        <td height="50">Table Data 2</td>
    </tr>
</table>
<br>

Code:

<br>

```html
<p>Basic one:</p>

<table>
    <tr>
        <th>Table Header 1</th>
        <th>Table Header 2</th>
    </tr>
    <tr>
        <td>Table Data 1</td>
        <td>Table Data 2</td>
    </tr>
</table>

<p>Modified one:</p>

<table bgcolor="black">
    <tr bgcolor="green" align="center" width="200">
        <th width="100">Table Header 1</th>
        <th width="100">Table Header 2</th>
    </tr>
    <tr bgcolor="lightgreen" align="center">
        <td height="50">Table Data 1</td>
        <td height="50">Table Data 2</td>
    </tr>
</table>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Colorful page
To make things colorful use attribute `style`. To add colors use <u title="black">text</u>, <u title="#000000">hex</u> or <u title="rgb(0, 0, 0)">rgb</u> values.

<br>

Check out [Website's page 3](https://terraboii.github.io/HTML_notes/page3.html "page 3").

<br>

Code (from page 3):

<br>

```html
<body style="background-color: black;">
    <a href="index.html"><h3 style="color: rgb(0, 255, 255);"><b>Go back to main page</b></h3></a>
    <p style="color: blue; font-size: 60px; background-color: #444444;"><b style="color: red;">R</b><i style="color: green;">G</i>B</p>
</body>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>

## Span and div
`span` tag - adds markup to text or portion of a document. \
`div` tag - defines a division of a document.

<br>
<div style="background-color: #666666;">
    <p>
        <span style="color:red;">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</span> Quasi fugiat deleniti tenetur. Adipisci ratione, repudiandae dolorem magni consectetur dolore libero unde velit est quod, delectus nesciunt. Consequuntur, dolore dolorum! Nostrum.
    </p>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo quas eveniet fugit laudantium officia quam quos cum, minima dolorum soluta blanditiis sed ut consequatur consectetur. Nostrum quidem eum maiores cupiditate!
    </p>
</div>
<br>

Code:

<br>

```html
<div style="background-color: #666666;">
    <p>
        <span style="color:red;">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</span> Quasi fugiat deleniti tenetur. Adipisci ratione, repudiandae dolorem magni consectetur dolore libero unde velit est quod, delectus nesciunt. Consequuntur, dolore dolorum! Nostrum.
    </p>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo quas eveniet fugit laudantium officia quam quos cum, minima dolorum soluta blanditiis sed ut consequatur consectetur. Nostrum quidem eum maiores cupiditate!
    </p>
</div>
```

<p align="right">(<a href="#top" title="to the top of the page">back to top</a>)</p><br>