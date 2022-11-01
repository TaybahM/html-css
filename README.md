# HTML Tags

## `<!--...-->`

**\<!--** This is a comment, comments are not displayed in the browser **-- >**

* Supported by all browsers
* In Javascript, two forward slashes are required to prevent JavaScript from attempting to execute the `-->` tag, for example:

> `<scipt type="text/javascript"`\
> `<!--`\
> `function displayMsg() {`\
> &#x20; `alert("Hello World!")`\
> `}`\
> `//-->`

* You can use comments to explain your code, which can help you when you edit the source code at a later date. This is especially useful if you have alot of code

## \<!Doctype html>

**\<!Doctype html>** All HTML documents must starts with a `<!Doctype>` declaration&#x20;

* Supported by all browsers
* Can be written in mutliple formats: \
  `<!DOCTYPE html>`\
  `<!DocType html>`\
  `<!<Doctype html>`\
  `<!doctype html>`

## \<a>

**\<a>** defines a hyperlink, which is used to link from one page to another

* Supported by all browsers
* must have a `href` attribute, or else it's just a placeholder for a hyperlink
* a linked page is normally displayed in the current browser window, unless specified&#x20;

Attributes

| Attribute      | Value                                                                                                                                                  | Description                                                                                                                                                                                 |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| download       | filename                                                                                                                                               | Specifies that the target will be downloaded when a user clicks on the hyperlink                                                                                                            |
| href           | URL                                                                                                                                                    | Specifies the URL of the page the link goes to                                                                                                                                              |
| hreflang       | language\_code                                                                                                                                         | Specifies the language of the linked document                                                                                                                                               |
| media          | media\_query                                                                                                                                           | Specifies what media/device the linked document is optimized for                                                                                                                            |
| ping           | lists\_of\_URLs                                                                                                                                        | Specifies a space-separated list of URLs to which, when the link is followed, post requests with the body ping will be sent by the browser (in the background). Typically used for tracking |
| referrerpolicy | <p>no-referrer<br>no-referrer-when-downgrade<br>origin<br>origin-when-cross-origin<br>same-origin<br>strict-origin-when-cross-origin<br>unsafe-url</p> | Specifies which referrer information to send with the link                                                                                                                                  |
| rel            | <p>alternate<br>author<br>bookmark<br>external<br>help<br>license<br>next<br>nofollow<br>noreferrer<br>noopener<br>prev<br>search<br>tag</p>           | Specifies the relationship between the current document and the linked document                                                                                                             |
| target         | <p>_blank<br>_parent<br>_self<br>_top</p>                                                                                                              | Specifies where to open the linked document                                                                                                                                                 |
| type           | media\_type                                                                                                                                            | Specifies the media type of the linked document                                                                                                                                             |

## \<abbr>

**\<abbr>** defines an abbreviation or an acronym

* Supported by all browsers
* Example: \
  `<abbr title="Cascading Style Sheets">CSS</abbr>`

## \<address>

**\<address>** defines the contact information for the author/owner of a document or article

{% tabs %}
{% tab title="Code" %}
{% code lineNumbers="true" %}
```html
<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```
{% endcode %}
{% endtab %}

{% tab title="Output" %}
Written by [Jon Doe](mailto:webmaster@example.com).\
Visit us at:\
Example.com\
Box 564, Disneyland\
USA
{% endtab %}
{% endtabs %}

* The contact information can be an email address, URL, physical address, phone number, social media handle, etc.&#x20;
* The text in `<address>` elements usually renders in _italic,_ and browsers will always add a line break before and after the `<address>` elelment by default
* Supported by all browsers
* Most browsers will display the `<address>` element with the following defaultvalues: \
  `address {`\
  &#x20; `display: block;`\
  &#x20; `font-style: italic;`\
  `}`
* ## \<area>

**\<area>** defines an area inside an image map (an image map is an image with clickable areas)

* Supported by all browsers
* The `<area>` element will always be nested inside a `<map>` tag
* The `usemap` attribute in `<img>` is associated with the `<map>` element's `name` attribute, and creates a relationship between the image and the map

Attributes

| Attribute      | Value                                                                                                                                 | Description                                                                         |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| alt            | text                                                                                                                                  | Specifies an alternate text for the area. Required if the href attribute is present |
| coords         | coordinates                                                                                                                           | Specifies the coordinates of the area                                               |
| donwload       | filename                                                                                                                              | Specifies that the target will be downloaded when a user clicks on the hyperlink    |
| href           | URL                                                                                                                                   | Specifies the hyperlink target for the area                                         |
| hreflang       | language\_code                                                                                                                        | Specifies the language of the target URL                                            |
| media          | media query                                                                                                                           | Specifies what media/device the target URL is optimized for                         |
| referrerpolicy | no-referrer, no-referrer-when-downgrade, origin, origin-when-cross-origin, same-origin , strict-origin-when-cross-origin , unsafe-url | Specifies which referrer information to send with the link                          |
| rel            | alternate, author, bookmark, help, license, next, nofollow, noreferrer , prefetch, prev, search, tag                                  | Specifies the relationship between the current document and the target URL          |
| shape          | default, rect, circle, poly                                                                                                           | Specifies the shape of the area                                                     |
| target         | \_blank, \_parent, \_self, \_top, framename                                                                                           | Specifies where to open the target URL                                              |
| type           | media\_type                                                                                                                           | Specifies the media type of the target URL                                          |

{% embed url="https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_areamap2" %}
See Example of AREA here
{% endembed %}

* Most browsers will display the `<area>` element with the followinf defaut values\
  `area {`\
  &#x20; `display: none;`\
  `}`

## \<article>

**\<article>** specifies independent, self-contained content&#x20;

* an article should make sense on its own and it should be possible to distribute it independently from the rest of the site&#x20;
* The `<article>`element does not render as anything special in a browser. However, you can use CSS to style the `<article>` element&#x20;

{% tabs %}
{% tab title="Code" %}
{% code lineNumbers="true" %}
```html
<!DOCTYPE html>
<html>
<head>
<style>
.all-browsers {
  margin: 0;
  padding: 5px;
  background-color: lightgray;
}

.all-browsers > h1, .browser {
  margin: 10px;
  padding: 5px;
}

.browser {
  background: white;
}

.browser > h2, p {
  margin: 4px;
  font-size: 90%;
}
</style>
</head>
<body>

<h1>The article element - Styled with CSS</h1>

<article class="all-browsers">
  <h1>Most Popular Browsers</h1>
  <article class="browser">
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
  </article>
  <article class="browser">
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
  </article>
  <article class="browser">
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
  </article>
</article>

</body>
</html>
```
{% endcode %}
{% endtab %}

{% tab title="Output" %}
{% embed url="https://codepen.io/Taybah/pen/mdKVLpz" %}
{% endtab %}
{% endtabs %}

* Browser Support

| Element    | Chrome | Edge | Firefox | Safari | Opera |
| ---------- | ------ | ---- | ------- | ------ | ----- |
| \<article> | 6.0    | 9.0  | 4.0     | 5.0    | 11.1  |
