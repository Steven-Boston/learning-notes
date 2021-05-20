# Reading 201-14(14a): Transforms, Transitions, and Animatons

## CSS Transforms
This article is available [here.](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

Transform is a feature new to CSS3, implemented with `transform: value(amt)`. Transform can require a vendor prefix to function in some browsers. 

### 2D Transforms:

- `transform: rotate(60deg);` for rotation
- `transform: scale(.8);` to rescale display. `scale(x,y)`, `scaleY()` and `scaleX` also work. 
- `translate(x,y)`, `translateX()`, and `translateY()` will move the subject in various directions. 
- `skewX(5deg)`, `skewY(-10deg)`, and `skew(xdeg, ydeg)` will distort the subject. 

These can be combined to acheive a variety of effects. Given no alteration, the changes will focus on the centerpoint of the block. This can be adjusted via `transform-origin: Xpx Ypx;`.

### 3D Transforms:

To make three-dimensional transformations, we require a perspective setting to be established. The perspective can be drawn either from individual elements of from parent elements in order to have a unified perspective. perspective depth is also a concern, and comes as the value in the perspective line: 

`transform: perspective(100px) rotateY(80deg);`

The origin of the perspective can also be offset via `perspective-origin:` just as with the 2d examples. The 3d tranformations come in the same forms, but with additional z-axis available for working with. 

## CSS Transitions
This article id available [here.](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)



## 8 Transitions Clickbait
View this exciting article with this one simple [link!](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)



# CSS Animation samples

Several links to sample animations were provided with this assignment, and I have included them below: 

- [6 Buttons Animated](https://codepen.io/retyui/pen/ByoaXV)
- [CSS3 Keyframes Animation](https://codepen.io/akshaychauhan/pen/oAfae)
- [Pure CSS Bounce Animation](http://codepen.io/dp_lewis/pen/gCfBv)
- [404 Animation](https://codepen.io/kieranfivestars/pen/MYdQxX)