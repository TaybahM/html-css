# Introduction

HTML is the standard markup language for creating simple to complex Web pages. HTML stands for Hyper Text Markup Language and is used to the descrip the structure of a page. Any website consists of a series of elements that tell the browser how to display content on their page.&#x20;

"Elements" or "tags" are used to label pieces of content. For example the `<p>` tag is used to organize text content into paragraph elements and the `<img>` tag is used to embed images into a page.&#x20;

Majority of the tags have an opening tag and a closing tag to wrap around content. closing tabs are denoted with a backslash like this: `</tag_name>`. HTML tags are not visible in the browser. The following diagram illustrates how tags are used in HTML elements:&#x20;

<figure><img src="https://assets.digitalocean.com/django_gunicorn_nginx_2004/articles/new_learners/html-element-diagram.png" alt=""><figcaption><p>www.digitalocean.com</p></figcaption></figure>

### HTML CSS JS

{% tabs %}
{% tab title="First Tab" %}
{% code lineNumbers="true" %}
```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```
{% endcode %}



* The `<!DOCTYPE html>` declaration defines that this document is an HTML5 document
* The `<html>` element is the root element of an HTML page and contains all the other HTML elements
* The `<head>` element contains meta information about the HTML page. The meta is the metadata about  the document and usually contains the title or style of the page. This information is not displayed on the web page
* The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
* The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
* The `<h1>` element defines a large heading
* The `<p>` element defines a paragraph
{% endtab %}

{% tab title="Second Tab" %}
## My First Heading

My first paragraph.
{% endtab %}
{% endtabs %}

HTML has many uses, such as web development, internet navigation and web documentation. It should also be noted that HTML is not considered a programming language as it cannot create dynamic functionality. A website created using just HTML would be static. HTML, CSS and JS usually work together to create a dynamic and functional website.

CSS stands for Cascading Style Sheets and is used alongside HTML. It tells HTML how to display elements on the screen. This coding language work side to side with HTML and is a rule-based language.&#x20;

JS stands for JavaScript and is used to enable dynamic interactivity on websites when its applied to an HTML document. Below is an example of what all three languages look like:

{% tabs %}
{% tab title="HTML" %}
```html
<!Doctype html>
<html>
<body>
<h1>I am a headline made with HTML</h1>
<p>And I am a simple text paragraph. The color of this text is styled with CSS. Click the button below to remove me through the power JavaScript.</p>
<button>Hide the text above</button>
</body>
</html>
```

Below is what this code does when it all works together
{% endtab %}

{% tab title="CSS" %}
```css
body {
	font-family: sans-serif;
	text-align: center;
	padding: 3rem;
	font-size: 1.125rem;
	line-height: 1.5;
	transition: all 725ms ease-in-out;
}

h1 {
	font-size: 2rem;
	font-weight: bolder;
	margin-bottom: 1rem;
}

p {
	margin-bottom: 1rem;
	color: tomato;
}

button {
	cursor: pointer;
	appearance: none;
	border-radius: 4px;
	font-size: 1.25rem;
	padding: 0.75rem 1rem;
	border: 1px solid navy;
	background-color: dodgerblue;
	color: white;
}
```
{% endtab %}

{% tab title="JS" %}
```javascript
$('button').on('click', function() {
	$('p').css('opacity', 0);
});
```
{% endtab %}
{% endtabs %}

{% embed url="https://codepen.io/rcyou/pen/QEObEZ" %}
Ryan Young - CodePen
{% endembed %}

#### BREAKING DOWN THE CSS
