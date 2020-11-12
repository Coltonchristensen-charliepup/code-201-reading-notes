# **css transforms, transitions and animations**

> Transforms: with CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, positions, and change elements. All of these new techniques are made possible by transform property. Which comes in two different settings, two-demensional and three dimensional. The actual syntax forum of the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

* Example: 
div{
  -webkit-transform: scale(1.5);
  -moz-transform: scale(1.5);
  -o-transform: scale(1.5);
  transform: (1.5);
}

* Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. 

* Example:
  * html: <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>

  * CSS: .box-1 {
    transform: rotate(20deg);
  }
  .box-2 {
    transform: rotate(-55deg);
  }

* 2d scale:

  * Example html&CSS: <figure class="box-1">Box 1</firgure>
  <figure class="box-2">Box 2</figure>

  .box-1{
    transform: scale(.75);
  }
  .box-2 {
    transform: scale(1.25);
  }

> 2D Cube Demo

* HTML

<div class="cube">
  <figure class="side top">1</figure>
  <figure class="side left">2</figure>
  <figure class="side right">3</figure>
</div>

                
* CSS

.cube {
  position: relative;
}
.side {
  height: 95px;
  position: absolute;
  width: 95px;
}
.top {
  background: #9acc53;
  transform: rotate(-45deg) skew(15deg, 15deg);
}
.left {
  background: #8ec63f;
  transform: rotate(15deg) skew(15deg, 15deg) translate(-50%, 100%);
}
.right {
  background: #80b239;
  transform: rotate(-15deg) skew(-15deg, -15deg) translate(50%, 100%);
}


> Transform Origin:

* HTML:

<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>
<figure class="box-3">Box 3</figure>
<figure class="box-4">Box 3</figure>

              
* CSS:

.box-1 {
  transform: rotate(15deg);
  transform-origin: 0 0;
}
.box-2 {
  transform: scale(.5);
  transform-origin: 100% 100%;
}
.box-3 {
  transform: skewX(20deg);
  transform-origin: top left;
}
.box-4 {
  transform: scale(.75) translate(-10px, -10px);
  transform-origin: 20px 50px;