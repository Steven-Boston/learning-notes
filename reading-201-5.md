# Readings 201-05: Images, Color, Text

## Duckett HTML/CSS 5: Images

Images form a critical part of most websites, and habdling them often requires specific approach. Images should generally be stored in their own folder for clear organization of website files. The image tag has a few useful attributes:
- src: necessary for linking the source of the image
- alt: adds a description of the image for when it cannot be displayed
- title: adds a title for the image that generally appears when it is hovered
- height/width: allows for inline coding that defines the dimensions of the image (probably better handled in CSS).

## Duckett HTML/CSS 11: Color
this section from 102-5:

Color in CSS can be applied to various elements. It can be specified in a few different ways: 
- RGB values in the form of `{color: rgb(100.100.100);}` 
- Hex Codes `{color: #ee3e80;}`
- Color names `{color: DarlCyan;}`
- `{background-color:` can be used to specify a section o f background color rather than the element itself
Contrast between foreground and background are critical for readability. `{opacity: 0.9;}` with the value between 0.0 and 1.0 will set opacity. 
CSS3 allows for HSL (hue, saturation, lightness) codes to identify colors in the form `: hsla(0,75%,95%,0.3)`, with the fourth value (a) being transparency. 

## Duckett HTML/CSS 12: Text
There are a small number of fonts that can be expected to be available on a user's computer, which effectively breakdown into five families:

- Serif: Georgia, Times New Roman
- Sans-Serif: Arial, Verdana, Helvetica
- MonoSpace: Courier, Courier New
- Cursive: Comic Sans, Monotype Corsiva,
- Fantasy (IMPACT, Haettenschwieler)
There are also a number of keys to use on text: 
- `font-family` allows one of these to be generally selected 
- `font-size` gives opportinities to adjust the size. 
- `font-weight: bold` sets bold
- `font-style:` normal, italic, or oblique
- `text-transform:` uppercase, lowercase, capitalize
- `text-decoration:` underline, overline, or strikethrough
- `line-height`adjusts the total height of lines of text
- `letter-spacing` and `word-spacing` give similar controls. 
- `text-align:` left, right, center, justify

Several other more niche keys for text are explained in Chapter 12.

## Rahul Nanwani: JPEG vs. PNG vs. GIF
This article can be found [here](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

Rahul has a lot to say about different image formats, but he hits us with a valuable TL:DR right away:

- JPEG should be used for photographs without sharply contrasting colors.
- PNG is the best option when an image needs to be made transparent of generally requires pronounced points of color definition. 
- GIF is for...   ...well it's for GIFs

This is because JPEG images support a full range of colors and have the best compression, but lose quality in the process. PNG files have no data loss, but do not compress nearly as small, which is exacerbated if using the PNG24 format rather than PNG8, which predictably is the only way to gain access to the full range of colors.

Of the above formats, only GIF supports animation. That's kinda the end of the story there.

And for this episode of reading notes, for that matter!


[<<Return to Home](README.md)