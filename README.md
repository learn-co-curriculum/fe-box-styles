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

<div style="color:white;width:50px;height:50px;background:url(http://placeimg.com/50/50/nature);margin-bottom: 20px;">Some text...</div>

Here are some common background properties and their accepted values seperated by `|` pipes.

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

### Vendor Prefixes

A quick note, many of the following examples below specify the same property three or more times using prefixes such as `-webkit-` or `-moz-`. These are browser vendor prefixes. When a new CSS feature comes into existence it takes time for all the different browsers to include support for the property. During this time while the vendor is adjusting support they will tag a prefix onto the beginning of the property so that it will only effect their specific browser. Eventually when all vendors provide universal support for a new property the prefixes are no longer needed. So when we see these prefixes it is only for supporting new features on older browser versions. As time goes on these vendor prefixes become less neccessary, however we have included them below for now, as at the time of writing this these were neccesary for these new properties to display the same across all browsers old and new.

### Border Radius

Border radius allows us to round the corners of elements. you can give it one value to uniformly round the edges on all sides or a second value following a `/` forward slash to adjust the radii to make squished curves, or give it up to four values to indicate different measurements for each of the four corners of the element in order top-left, top-right, bottom-right, bottom-left.

```css
div {
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  border-radius: 20px;
}
```

<div style="width:50px;height:50px;background:#ccc;border-radius:20px;-webkit-border-radius:20px;-moz-border-radius:20px;"></div>

Where as `border-radius` is a shorthand property we can also call out each corner using individual properties such as: `border-top-left-radius`, `border-top-right-radius`, `border-bottom-right-radius`, `border-bottom-left-radius`.

### Box Shadow

Bow shadow adds a nice drop shadow aurrounding the element. It is cast outside the border into the margin area of the element. It is defined using three values: the first being horizontal offset, followed by vertical offset, feather, and color. The offsets  push the sadoes out and away from the element. The feather softens the shadow, and the color sets the hue.

```css
div {
  -webkit-box-shadow: 5px 5px 10px #888;
  -moz-box-shadow: 5px 5px 10px #888;
  box-shadow: 5px 5px 10px #888;
}
```

<div style="width:50px;height:50px;background:#ccc;box-shadow: 5px 5px 10px #888;-moz-box-shadow: 5px 5px 10px #888;-webkit-box-shadow: 5px 5px 10px #888;"></div>

### Opacity

Opacity allows us to add transparency to our elements. The standard `opacity` property uses vlaues 0 to 1, with 0 being completely transparent and 1 being completely opaque. 0.5 for example, is the equivalent of 50% opacity.

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

Using the background property we can also supply gradient tones. This is done by providing position or angle information for where the first color starts, followed by the color stop value, then optionally followed by a percent of space within the element that color stop should take up. There are three types of color gradients `linear-gradient`, `radial-gradient`, and repeating: `repeating-linear-gradient` and `repeating-radial-gradient`. below is an example of a linear gradient.

```css
div {
  background: -moz-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);
  background: -webkit-gradient(left top, right top, color-stop(0%, rgba(94,250,255,1)), color-stop(100%, rgba(3,22,237,1)));
  background: -webkit-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);
  background: -o-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);
  background: -ms-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);
  background: linear-gradient(to right, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#5efaff', endColorstr='#0316ed', GradientType=1 );
}
```

<div style="width:50px;height:50px;background: -moz-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);background: -webkit-gradient(left top, right top, color-stop(0%, rgba(94,250,255,1)), color-stop(100%, rgba(3,22,237,1)));background: -webkit-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);background: -o-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);background: -ms-linear-gradient(left, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);background: linear-gradient(to right, rgba(94,250,255,1) 0%, rgba(3,22,237,1) 100%);filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#5efaff', endColorstr='#0316ed', GradientType=1 );"></div>

## Summary

- ...

## Resources

- [Presentation Slides](https://docs.google.com/presentation/d/1NIXi8WE9PfQtYgAnFhCRQ64RK_cw2hDT2sUeG4puLuo/edit?usp=sharing)
- [Box Style - Code Example](http://jsfiddle.net/flatiron_school/wsNXW/1/)
- [Online Gradient Generator](http://www.colorzilla.com/gradient-editor/)
- [MDN - CSS - Background](https://developer.mozilla.org/en-US/docs/Web/CSS/background)

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/fe-box-styles' title='CSS Box Styles ~ 20min'>CSS Box Styles</a> on Learn.co and start learning to code for free.</p>
