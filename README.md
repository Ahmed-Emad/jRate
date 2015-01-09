
jRate - Rating jQuery plugin
=================

This jquery plugin helps to generate RATING with various features. Download and include this plugin in your html file.

![Demo](https://rawgit.com/senthilporunan/jRate/master/images/jRate-Star-Demo.gif)

### Including it on your page

Include jQuery and this plugin on your page.
```
<script src="jRate.js"></script>

```
### Basic Usage
```
<div id="jRate"></div>
$("#jRate").jRate();
```
#Features
###Start Color and End Color

Set your favourite start and end color. By giving value in the form of hex value, rgb value or standard color name. We can use one color format also by giving same start and end color.

```js
$("#jRate").jRate({
  startColor: "cyan",
  endColor: "blue"
});
```
###Width and Height
We can customize our own value for width and height.
```js
$("#jRate").jRate({
  width: 70,
  height: 70
});
```
####Shape
We can chooose shape from available list. If you need more shapes, raise feature request in github. Available shapes are STAR, RECTANGLE, SQUARE, CIRCLE, RHOMBUS, TRIANGLE.
```js
$("#jRate").jRate({
  shape: 'RHOMBUS'
});
```
####Width and Height Growth
Make the shapes from smaller to bigger. We can use growth field to make this happen.
```js
$("#jRate").jRate({
  widthGrowth: 0.2,
  heightGrowth: 0.2
});
```

####Count
Number of shapes was decided by the count parameter. We can customize own numeric value for it.
```js
$("#jRate").jRate({
  count: 10
});
```
####Background Color
Set your favourite background color. By giving value in the form of hex value, rgb value or standard color name.
```js
$("#jRate").jRate({
  backgroundColor: 'black'
});
```
####Gap
We can set our own gap between two shapes. We can customize our own values in it.
```js
$("#jRate").jRate({
  shapeGap: '10px'
});
```
####Opacity
Set opacity value.
```js
$("#jRate").jRate({
  opacity: 0.3
});
```

####Minimum and Maximum Value
Set a desired minimum and maximum value.
```js
$("#jRate").jRate({
  min: 10,
  max: 15
});
```
####Precision
Set the precision value.
```js
$("#jRate").jRate({
  precision: 0
});
```
####Horizontal
We can set a boolean variable to make horizontal or vertical. And, set a boolean value for reverse.
```js
$("#jRate").jRate({
  horizontal: false
});
```
####Reverse
We can set a boolean variable to make reverse or not.
```js
$("#jRate").jRate({
  reverse: true
});
```
####ReadOnly
Set the readonly value.
```js
$("#jRate").jRate({
  readOnly: true
});
```
####onChange
Write your own methods to do own action when the rating value change action occurs.
```js
$("#jRate").jRate({
  onChange: function(rating) {
    $('#demo-onchange-value').text("Your Rating: "+rating);
  }
});
```
####onSet
Write your own methods to do own action when the rating value click or set action occurs.
```js
$("#jRate").jRate({
  onSet: function(rating) {
    $('#demo-onset-value').text("Selected Rating: "+rating);
  }
});
```
####License
This plugin is licensed under the [MIT license](https://github.com/senthilporunan/jRate/blob/master/LICENSE).
Copyright (c) 2015 [Senthil Porunan](http://www.toolitup.com/)
