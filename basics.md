---
description: Basic HTML Examples to get your page started
---

# Basics

## HTML Documents

All HTML documents must start with a document type declaration: `<!DOCTYPE html>`, the HTML document itself begins with an `<html>` tag and ends with `</html>`. The visible portion of the HTML document, lays inbetween `<body>` and `</body>`.&#x20;

{% tabs %}
{% tab title="Code" %}
{% code lineNumbers="true" %}
```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```
{% endcode %}

In this example, the `<h1>` tag tells HTML that the text written in between `<h1>` and `</h1>` should be formatting as a heading.&#x20;
{% endtab %}

{% tab title="Output" %}
## My First Heading

My first paragraph.
{% endtab %}
{% endtabs %}

HTML has pre-formatted heading sizes that go from 1-6. 1 being the largest and 6 being the smallest. This allows users to create multiple subheadings within each other with ease. In the example below, headings 1-3 are used.

{% tabs %}
{% tab title="Code" %}
{% code lineNumbers="true" %}
```html
<!DOCTYPE html>
<html>
<body>

<h1>Title</h1>
<p>Paragraph 1</p>
<h2>Sub-title</h2>
<p>Paragraph 2</p>
<h3>Sub to the Sub-title</h3>
<p>Paragraph 3</p>

</body>
</html>
```
{% endcode %}
{% endtab %}

{% tab title="Output" %}
## Title

Paragraph 1

### Sub-title

Paragraph 2

#### Sub to the Sub-title

Paragraph 3
{% endtab %}
{% endtabs %}
