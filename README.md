# Introduction

HTML is the standard markup language for creating simple to complex Web pages. HTML stands for Hyper Text Markup Language and is used to the descrip the structure of a page. Any website consists of a series of elements that tell the browser how to display content on their page.&#x20;

"Elements" or "tags" are used to label pieces of content. For example the `<p>` tag is used to organize text content into paragraph elements and the `<img>` tag is used to embed images into a page.&#x20;

Majority of the tags have an opening tag and a closing tag to wrap around content. closing tabs are denoted with a backslash like this: `</tag_name>`. HTML tags are not visible in the browser. The following diagram illustrates how tags are used in HTML elements:&#x20;

<figure><img src="https://assets.digitalocean.com/django_gunicorn_nginx_2004/articles/new_learners/html-element-diagram.png" alt=""><figcaption><p>www.digitalocean.com</p></figcaption></figure>

### HTML CSS JS

{% tabs %}
{% tab title="Code" %}
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
* The `<head>` element contains meta information about the HTML page. The meta is the metadata about  the document and usually contains the title or style of the page. It can also be a place where HTML can link to a CSS style sheet for design, you will see what this is in a moment. This information is not displayed on the web page
* The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
* The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
* The `<h1>` element defines a large heading
* The `<p>` element defines a paragraph
{% endtab %}

{% tab title="Output" %}
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

### CSS Breakdown

CSS is used to defines styles for you web pages, including designs, layout and variations in display for different devices and screen sizes. HTML itself was never created to contain tags for website formatting. It was simply created to display contents of a web page for everyone to see. Once designers began attempting to include tags like `<font>` to format the font into HTML it became a coding nightmare for web developers. Large websites where fonts and color information were added to every single page began causing issues and creating long, expensive and unnecessary design projects.&#x20;

#### Internal Stylesheet

CSS can be added to a web page as an internal style sheet, external stylesheet or inline the HTML text. An internal stylesheet resides within an HTML document. To create this, we can place our CSS in between the `<style>` tag which is inside the HTML `<head>`tag. An internal stylesheet is best when there isn't much CSS used in a web page. Once the page gets larger and more complex, it requires more CSS. In that case, it's best to have a seperate page containing just the CSS information that links straight to the main HTML document, that would then be called the external stylesheet. Below is an example of an internal styelsheet:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My CSS experiment</title>
    <style>
      h1 {
        color: blue;
        background-color: yellow;
        border: 1px solid black;
      }

      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```

In this example, we can see the CSS begin right under the `<style>` tag and end as soon as that tag ends. In it the `<h1>` and `<p>` tags are being formatted. Let's break down each part of the `h1` selector:&#x20;

```css
h1 {
        color: blue;
        background-color: yellow;
        border: 1px solid black;
      }
```

* `h1` This is the selector, it points to the HTML element you want to style
* `{}` A declaration begins at the start of a bracket and ends at the end of it
* `color:` This is called the property and tells HTML the color of `h1`
* `blue;` This is the value and tells HTML that the color of `h1` is blue
* `background-color: yellow;` This portion tells HTML that the background of the document will be yellow. In place of the word yellow, you can also put hex codes to specify the color you would like

{% hint style="info" %}
**HEX Colors** are specified with #RRGGBB, where RR (red), GG(green) and BB(blue) hexadecimal integers specify the components of the color. [Read more about Hex Colors](https://opusdesign.us/wordcount/what-are-hex-codes-for-colors/).
{% endhint %}

#### External Stylesheet

An external stylesheet contains CSS in a seperate file with a `.css` extension. This is the most common, useful and recommended method of bringing CSS into an HTML document. You can reference an external CSS stylesheet from an HTML `<link>` element:&#x20;

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My CSS experiment</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```

In this example there is a link created for a seperate CSS stylesheet that is titled "`styles.css`". "rel" tells HTML that there is a relationship between the HTML document and a stylesheet. The files may look like this:&#x20;

{% tabs %}
{% tab title="index.html" %}
```html
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```
{% endtab %}

{% tab title="styles.css" %}
```css
h1 {
  color: blue;
  background-color: yellow;
  border: 1px solid black;
}

p {
  color: red;
}
```
{% endtab %}

{% tab title="Output" %}
{% embed url="https://codepen.io/Taybah/pen/rNKLBLm" %}
Taybah Mohammad - CodePen
{% endembed %}
{% endtab %}
{% endtabs %}

In this example, the tabs have been titled with the appropriate file name. index.html is the most common name used for the landing page in an HTML webpage. It other words, index.html is used for the homepage.&#x20;

#### Inline CSS

Inline CSS affect a single HTML element at a time. This may look like:&#x20;

```html
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
  </head>
  <body>
    <h1 style="color: blue;background-color: yellow;border: 1px solid black;">
      Hello World!
    </h1>
    <p style="color:red;">This is my first CSS example</p>
  </body>
</html>
```

**Avoing CSS in this way**, this is the least efficient way to use CSS in a an HTML page. Seperating code in between the `<style>` tags or in a seperate page make it easier to read code and work through it.&#x20;

### Exercise

Now we will work on a webpage with an [external stylesheet](./#external-stylesheet) Create a folder on your computer and name it whatever you like. Inside the folder, create a text file and paste the following code inside (you can use notepad to do this or any [text editor software](https://www.g2.com/categories/text-editor) you would like):

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiments</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p>Create your test HTML here</p>
  </body>
</html>
```

Save the file as `"index.html"`. Navigating to the folder and clicking on the file will open it up in your browser. For now it should just say "Create your test HTML here". The title of the page should say "My CSS expiriments". Remember that the `<title>` tag will display whatever is on the browser's title bar or in the page's tab.

Now we can add our css file and title it `"styles.css"`. In this file, paste the following:&#x20;

```
p {
  color: red;
}
```

After you've completed these steps, reload the index.html page and the text should now appear red. That is becuase your HTML page is linked to the CSS page, and your code tells the browser to render the text in that color.



