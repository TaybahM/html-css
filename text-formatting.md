---
description: HTML Text Formatting
---

# Text Formatting

HTML facilitates the ability for formatting text just like we do in MS Word or any other text editing software. In the following examples, the comment tag is used. A comment tag allows web developers to add extra information that stays hidden for the viewers. It is usually used when the code gets too complex.&#x20;

### Bold, Small, Highlight, Italic

{% tabs %}
{% tab title="Code" %}
{% code lineNumbers="true" %}
```html
<!DOCTYPE html>
<html>
  
<body>
    <h2>Text Formatting</h2>
      
    <!--Bolded text-->
    <strong>Hello World</strong>
    <br>
      
    <!--Small text-->
    <small>Hello World</small>
    <br>
      
    <!--Highlighted text-->
    <mark>Hello World</mark>
    <br>

    <!--Italicized text-->
    <i>Hello World</i>
</body>
  
</html>
```
{% endcode %}
{% endtab %}

{% tab title="Output" %}
### Text Formatting

**Hello World**\
Hello World\
<mark style="background-color:yellow;">Hello World</mark>\ <mark style="background-color:yellow;"></mark>_Hello World_
{% endtab %}
{% endtabs %}

In this example the following tags were used:&#x20;

* `<strong>`: Tells the browser to render the contents in between as bolded words, which can be seen when clicking on the "output" tab above. The`<b>`tag can also be used with a similar effect.
* `<small>`: Defines smaller text, can be used for copyright text or side-comments - (Gitbooks cannot run this tag without extra external stylesheets, which is why the browser has not rendered it correctly. Copy and pasting the HTML from the "code" tab into [CodePen](https://codepen.io/Taybah/pen/LYrNjyL) will do the trick)&#x20;
* `<mark>`: Defines text that should be marked or highlighted. Generally the browser will render the contents within the `<mark>` tag as text with a yellow background
* `<i>`: Used to italicise text. The tag `<em>`can also be used with a similar effect.&#x20;
* `<br>`: some elements do not have end tags becuase they do not contain content. This tag for exampl, is used to tell the browser that there is a line break in between two seperate tags. Without this tag, the content would all be in a single line.&#x20;

{% hint style="info" %}
**CodePen**: "CodePen is an online community for testing and showcasing user-created HTML, CSS and JavaScript code snippets. It functions as an online code editor and open-source learning environment, where developers can create code snippets, called "pens," and test them.", This is a great place for beginners to test their code and play around with tags and elements.
{% endhint %}

### Paraghraph, Superscripts & Subscripts

{% tabs %}
{% tab title="Code" %}
{% code lineNumbers="true" %}
```html
<!DOCTYPE html>
<html>
  
<body>
    <h2>Text Formatting 2</h2>
      
    <!--Paragraph text-->
    <p>Hello World</p>
    <br>
      
    <!--Superscript text inside of a paragraph-->
    <p>Hello World<sup>superscript</sup></p>
    <br>
      
    <!--Subscript text inside of a paragraph-->
    <p>Hello World<sub>subscript</sub></p>
    <br>
</body>
  
</html>
```
{% endcode %}
{% endtab %}

{% tab title="Output" %}
{% embed url="https://codepen.io/Taybah/pen/KKezOBP" %}
Taybah Mohammad - CodePen
{% endembed %}
{% endtab %}
{% endtabs %}

In this example the following tags were used:&#x20;

* `<p>` : Defines a paragraph. The browser will automatically add a single blank line before and after each `<p>` element
* `<sup>`: Defines superscript text that is sometimes used for footnotes, like $$WWW^1$$
* `<sub>`: Defines subscript text that is sometimes used for chemical formulas, like $$H_2O$$

### Deleting and Inserting

{% tabs %}
{% tab title="Code" %}
```
<!DOCTYPE html>
<html>
  
<body>
    <h2>Text Formatting 3</h2>
      
    <!--Inserting-->
    <p>My favorite color is <del>blue</del> red.</p>
    <br>
    
    <!--Deleting-->
    <p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
    <br>
    
</body>
  
</html>
```
{% endtab %}

{% tab title="Output" %}
### Text Formatting 3

My favorite color is ~~blue~~ red.\
My favorite color is ~~blue~~ red.
{% endtab %}
{% endtabs %}

GitBooks does not render underlined text, in the third line in the "output" tabs, the text "red" should be underlined.

#### Simple Tags

|    Tag    |    Defenition    |
| :-------: | :--------------: |
|    \<b>   |     bold text    |
| \<strong> |  important text  |
|    \<i>   |    italic text   |
|   \<em>   |  emphasized text |
|  \<mark>  |    marked text   |
|  \<small> |   smaller text   |
|   \<del>  |   deleted text   |
|   \<ins>  |   inserted text  |
|   \<sub>  |  subscript text  |
|   \<sup>  | superscript text |
