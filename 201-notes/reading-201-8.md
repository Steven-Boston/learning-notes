# Duckett HTML/CSS 15: Layout

I did an overview of this chapter in reading 201-4, so I will be working form those notes and adding some detail here. 

This chapter concerns itself with the thorny business of layout in CSS, from basic positioning of different elements all the way to different overall design strategies. 

Boxes are either **block-level** or **inline**. A box within another is said to contained by that box. There are several methods of controlling this paradigm:
- Normal Flow: `position:static` block elements each occupy their own line, appearing in a single column 
- Relative Positioning: `position: relative` normal positioning with manual adjustments to individual elements
- Absolute Positioning: `position: absolute` The position of the element is strictly defnined and ignores other elements on the page
- Fixed Positioning: `position: fixed` positioning relative to the browser window and nothing else
- Floating Elements: `float: direction` one element floats in a position, and other content bends around it. 
`z-index` allows the developer to control which elements belong on top when they overlap
- `clear: ` (left, right, or both) allows one to set a box to float such that no content in the same container is touching it on one or both sides. 
- If all elements in a conatainer are floated, the container will sometimes not maintain its shape. This can be prevented by manually setting the width and setting `overflow: auto` to the container. 

This chapter also discusses screen sizes and their impact on webpage design. Since screen sizes range from 27 or more inch monitors all the way down to mobile devices of only a few inches, adjusting for this wide variation can be complex. 

Layouts can be setup with either fixed or liquid dimensions in mind. Fixed layouts use hard dimensions, and liquid use percentile values that adjust with the page. 

Grid layout is a useful tool for composition in webpage design. There are a few common grids with 960px width shown on pages 389-90.

[<<Return to Home](../README.md)



