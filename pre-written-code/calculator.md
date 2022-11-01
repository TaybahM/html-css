# Calculator

## HTML

{% code lineNumbers="true" %}
```html
<body>
  
  <div class="calculator">
    <div class="displayContainer"></div>
    <div class="buttonsContainer">
      <div class="button">1</div>
      <div class="button">2</div>
      <div class="button">3</div>
      <div class="button"id="operators"><b>×</b></div>
      <div class="button">4</div>
      <div class="button">5</div>
      <div class="button">6</div>
      <div class="button"id="operators"><b>÷</b></div>
      <div class="button">7</div>
      <div class="button">8</div>
      <div class="button">9</div>
      <div class="button"id="operators"><b>+</b></div>
      <div class="button">.</div>
      <div class="button">0</div>
      <div class="button"id="operators"><b>^</b></div>
      <div class="button"id="operators"><b>-</b></div>
      <div class="button"id="operators">AC</div>
      <div class="button"id="operators">C</div>
      <div class="equal"id="operators">=</div>
    </div>
  </div>

</body>
```
{% endcode %}

## CSS

{% code lineNumbers="true" %}
```css
html{
	height: 100%;
	width: 100%;
	background: #33343fff;
}
body{
	height: 100%;
	width: 100%;
  	background: blue;
  	margin: 0px;
  	display: flex;
  	justify-content: center;
  	align-items: center;
}


.calculator{
	background: #595a6eff;
    height: 500px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 20px;
    border-radius: 5%;
    box-shadow: 1px 5px 0px 21px black;, 13px 13px 25px;
}

.displayContainer{
	height: 100px;
	width: 350px;
	background: #173f15ff;
}

.buttonsContainer{
	height: 320px;
	width: 350px;
	background: #595a6eff;
	display: flex;
	flex-wrap: wrap;
	justify-content: center;
	align-items: center;
}

.button{
	background: white;
    font-family: Arial, Helvetica, sans-serif;
    height: 35px;
    width: 55px;
    border-radius: 100%;
    margin: 12px;
    align-items: center;
    justify-content: center;
    display: flex;
    user-select: none;
    font-size: 25px;
    color: black;
    box-shadow: 1px 12px 0px #33343fff, 1px 13px 25px white;
    font-weight: 500;
    border-style: double;
    border-color: #919191ff;
    flex-shrink: 0;
}

#operators{
	background: #919191ff;
	color: white;
}

.equal{
	background: white;
	height: 41px;
    width: 150px;
	border-radius: 50%;
	margin: 12px;
	align-items: center;
	justify-content: center;
	display: flex;
	user-select: none;
	font-size: 30px;
	color: #919191ff;
	box-shadow: 1px 12px 0px #33343fff, 1px 13px 25px white;
	font-size: 50px;
	font-weight: 600;
	border-style: double;
    border-color: #33343fff;
}

.equal:active{
	background: red;
	color: blue;
	box-shadow: 1px 1px 0px #33343fff, 13px 13px 25px #33343fff;
	margin-bottom: 0px;
	transition-duration: 0.07s;
}

.button:active{
	background: #b1b1b1ff;
	color: black;
	box-shadow: 1px 1px 0px #2f2f2fff, 13px 13px 25px #2f2f2fff;
	margin-top: 30px;
	margin-bottom: 0px;
	transition-duration: 0.07s;
}
```
{% endcode %}

{% embed url="https://codepen.io/Taybah/pen/JjZPMbQ" %}
