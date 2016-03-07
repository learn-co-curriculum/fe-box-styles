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

`background-color: black | #000 | rgba(0,0,01)`

`background-image: url(myimage.jpg)`

`background-position: top left | top center | top right `

`background-repeat: repeat | repeat-x | repeat-y | no-repeat`

`background-scroll: fixed | scroll`

`background-size: 100% | 1px | 1em | contain | cover`

`background: white url(myimage.jpg) no-repeat`

### Border

`border-size: 1% | 1px | 1em`

`border-color: blue | #00f | rbga(0,0,255,1)`

`border-style: solid | dashed | dotted | double | groove | ridge | inset | outset`

`border: 1px solid #000`

### Border Radius

```css
div {
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  border-radius: 20px;
}
```

### Box Shadow

```css
div {
  -webkit-box-shadow: 5px 5px 10px #888;
  -moz-box-shadow: 5px 5px 10px #888;
  box-shadow: 5px 5px 10px #888;
}
```

### Opacity

```css
div {
  filter: alpha(opacoty=50); /*IE*/
  -moz-opacity: 0.5; /*FF 0.9*/
  -khtml-opacity: 0.5; /*Safari 1.x*/
  opacity: 0.5;
}
```

### Gradient

...

## Summary

- ...

## Resources

- [Presentation Slides](https://docs.google.com/presentation/d/1NIXi8WE9PfQtYgAnFhCRQ64RK_cw2hDT2sUeG4puLuo/edit?usp=sharing)
- [Box Style - Code Example](http://jsfiddle.net/flatiron_school/wsNXW/1/)
- [Online Gradient Generator](http://www.colorzilla.com/gradient-editor/)

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/fe-box-styles' title='CSS Box Styles ~ 20min'>CSS Box Styles</a> on Learn.co and start learning to code for free.</p>
