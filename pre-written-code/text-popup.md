---
description: HTML, CSS & JS
---

# Text Popup

## HTML

{% code lineNumbers="true" %}
```html
<html lang="en">
<head>
     <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-9741419733823699"
     crossorigin="anonymous"></script>
<meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Untitled</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/ionicons/2.0.1/css/ionicons.min.css">
    <link rel="stylesheet" href="assets/css/style.css">
<link href="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css" rel="stylesheet" id="bootstrap-css">
<script src="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<title>Anchorheart</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="author" content="Taybah Mohammad">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<!-- Content for POPUP  -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
</head>

<center>
<div class="center hideform">
    <button id="close" class="button button3" style="float: right;">Hide</button>
    <p><b>DISCLAIMER:</b> The volunteers of Anchorheart are not professionals of any kind. We offer non crisis emotional support and companionship. If you are in crisis or need a licensed professional, please find professionals or crisis resources. Opinions expressed by volunteers aren’t necessarily the view or mission of Anchorheart.</p>
    <button class="button button3" align="center" onclick="window.location.href='https://docs.google.com/forms/d/e/1FAIpQLSfV7nt3ZnkWt93LNn3BzAy0DS60glPoKHDrtV9xYKqpdZCVqQ/viewform';" >I Understand & I wish to proceed</button>
</div>
<button id="show" align="center" class="button button3" >Form</button>
</center>
</html>
```
{% endcode %}

## CSS

{% code lineNumbers="true" %}
```css
.center {
    margin: auto;
    width: 60%;
    padding: 20px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

.hideform {
    display: none;
}


.button1 {
  background-color: white;
  color: black;
  border: 2px solid #4CAF50;
}

.button1:hover {
  background-color: #4CAF50;
  color: white;
}

.button2 {
  background-color: white;
  color: black;
  border: 2px solid #008CBA;
}

.button2:hover {
  background-color: #008CBA;
  color: white;
}

.button3 {
  background-color: white;
  color: black;
  border: 1px solid #3179cc;
}

.button3:hover {
  background-color: #3179cc;
  color: white;
}
```
{% endcode %}

## JavaScript

{% code lineNumbers="true" %}
```javascript
$('#show').on('click', function () {
    $('.center').show();
    $(this).hide();
})

$('#close').on('click', function () {
    $('.center').hide();
    $('#show').show();
})
```
{% endcode %}

****\
****\
****
