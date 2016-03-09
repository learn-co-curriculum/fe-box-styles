# CSS Box Styles

## Overview

In this lesson we will look at css properties for styling our boxes. We will cover background, box-shadow, gradients, opacity, and border-radius.

## Objectives

1. Apply background adjustments to color, image, gradients, and positioning.
2. Apply box shadows.
3. Apply border radius.
4. Apply opacity.

## Styling Box Elements

<iframe width="640" height="480" src="https://www.youtube.com/embed/T2AEbixxGRM?rel=0" frameborder="0" allowfullscreen></iframe>

*Note: Slides for this lecture video are provided in the resources at the bottom of this lesson.*

### Background

A quick way to breathe life into our layouts is to apply some colors, textures, and images into our backgrounds. Below are some commonly used background properties that will help our elements look great! When adding a background image, we can still easily place text and media content on top of it.

<div style="width:50px;height:50px;background:url(http://placeimg.com/50/50/animals)">Some text on top of our image!</div>

`background-color: black | #000 | rgba(0,0,01)`

Background color will fill the element a solid color, and accepts color name, hexidecimal, or rgb values. This color will fill edge to edge up until the border area.

`background-image: url(myimage.jpg)`

Background images allow us to fill our elements with photos, tectures, patterns, just about any visual you come across. we use the `url()` to point to our image file. Accepted formats include: jpg, gif, and png.

`background-position: top left | 50% 50% | 100px -30px`

Background position allows us to reposition our images inside of our element. We can supply directions such as top left, top right, top center, center, bottom left, bottom center, and bottom right. We can also provide (%) percents or (px) pixels measurements where the first value is the horizontal positioning and the second is vertical positioning. 

`background-repeat: repeat | repeat-x | repeat-y | no-repeat`

We can control whether or not our background image appears once or repeats. Repeating can be useful to tile patterns or textures.

`background-scroll: fixed | scroll`

Background scroll defines if the image should stay `fixed` in place while scrolling or if it should `scroll` with the content.

`background-size: 100% | 1px | 1em | contain | cover`

Background size allows us to set the size of the image in (%) percents of its element container, (px) exact pixels, or whether to `contain` itself within the dimesions of the element, or `cover` which causes it to cover the element edge to edge by cropping the image if neccesary.

`background: white url(myimage.jpg) no-repeat`

The shorthand property `background` allows us to give values for color, image, position, size, repeat, and attachment among others.

### Border

Border properties allow us to create a line at te edge of our element, below are a few key porperties and their accepted values separated by `|` pipes.

`border-size: 1% | 1px | 1em`

Border size allows us to se the thickness of the border in percents, pixels, or ems.

`border-color: blue | #00f | rbga(0,0,255,1)`

Border color allows us to set the color of our border using color names, hexidecimal, or rgb.

`border-style: solid | dashed | dotted | double | groove | ridge | inset | outset`

Border style allows us to alter the apperance of the border. Here we can see the different styles below in stunning blue,

<table>
  <tr>
    <th>Value</th><th>Example</th>
  </tr>
  <tr>
    <td>solid</td>
    <td><div style="width:50px;height:50px;border:4px solid blue;"></div></td>
  </tr>
  <tr>
    <td>dashed</td>
    <td><div style="width:50px;height:50px;border:4px dashed blue;"></div></td>
  </tr>
  <tr>
    <td>dotted</td>
    <td><div style="width:50px;height:50px;border:4px dotted blue;"></div></td>
  </tr>
  <tr>
    <td>double</td>
    <td><div style="width:50px;height:50px;border:4px double blue;"></div></td>
  </tr>
  <tr>
    <td>groove</td>
    <td><div style="width:50px;height:50px;border:4px groove blue;"></div></td>
  </tr>
  <tr>
    <td>ridge</td>
    <td><div style="width:50px;height:50px;border:4px ridge blue;"></div></td>
  </tr>
  <tr>
    <td>inset</td>
    <td><div style="width:50px;height:50px;border:4px inset blue;"></div></td>
  </tr>
  <tr>
    <td>outset</td>
    <td><div style="width:50px;height:50px;border:4px outset blue;"></div></td>
  </tr>
</table>

`border: 1px solid #000`

The shorthand property `border` allows us to set all of the properties in a single place.

### Border Radius

```css
div {
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  border-radius: 20px;
}
```

<div style="width:50px;height:50px;background:#ccc;border-radius:20px;-webkit-border-radius:20px;-moz-border-radius:20px;"></div>

### Box Shadow

```css
div {
  -webkit-box-shadow: 5px 5px 10px #888;
  -moz-box-shadow: 5px 5px 10px #888;
  box-shadow: 5px 5px 10px #888;
}
```

<div style="width:50px;height:50px;background:#ccc;box-shadow: 5px 5px 10px #888;-moz-box-shadow: 5px 5px 10px #888;-webkit-box-shadow: 5px 5px 10px #888;"></div>

### Opacity

```css
div {
  filter: alpha(opacity=50); /*IE*/
  -moz-opacity: 0.5; /*FF 0.9*/
  -khtml-opacity: 0.5; /*Safari 1.x*/
  opacity: 0.5;
}
```
<div style="width:50px;height:50px;background:aqua;"></div>
<div style="width:50px;height:50px;background:#ccc;filter: alpha(opacity=50);-moz-opacity: 0.4;-khtml-opacity: 0.5;opacity: 0.5;position:relative;z-index:1;top: -25px; left: 25px;"></div>

### Gradient

...

## Summary

- ...

## Resources

- [Presentation Slides](https://docs.google.com/presentation/d/1NIXi8WE9PfQtYgAnFhCRQ64RK_cw2hDT2sUeG4puLuo/edit?usp=sharing)
- [Box Style - Code Example](http://jsfiddle.net/flatiron_school/wsNXW/1/)
- [Online Gradient Generator](http://www.colorzilla.com/gradient-editor/)
- [MDN - CSS - Background](https://developer.mozilla.org/en-US/docs/Web/CSS/background)

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/fe-box-styles' title='CSS Box Styles ~ 20min'>CSS Box Styles</a> on Learn.co and start learning to code for free.</p>
