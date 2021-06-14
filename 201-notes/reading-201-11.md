# Reading 201-11: Audio, Video, Images, (Disco)

## Duckett HTML/CSS 16: Images

This chapter overviews selectors specific to images in CSS, and also gives some design tips for handling their design and placement in terms of contrast. 

## Duckett HTML/CSS 19: Practical Information

Chapter 19 could reasonably be called "Page Logistics," and spends most of its pages discussing search engine optimization, from keywords to the various arenas in which they can be deployed. 

## MDN: Video and Audio APIs
This article can be found [here.](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs)

`<video>` and `<audio>` elements are available in HTML to allow the developer to embed their namesakes into web pages. The controls element will add default browser controls for the videos player, but these are inconsistent, so building controls in is preferable. 

HTMLMediaElement API has options that can streamline this process. The article offers a sample file for the purpose, the contents of which I will copy here to take notes on: 
```html
<div class="player">
  <video controls>
    <source src="video/sintel-short.mp4" type="video/mp4">
    <source src="video/sintel-short.webm" type="video/webm">
    <!-- fallback content here -->
  </video>
  <div class="controls">
    <button class="play" data-icon="P" aria-label="play pause toggle"></button>
    <button class="stop" data-icon="S" aria-label="stop"></button>
    <div class="timer">
      <div></div>
      <span aria-label="timer">00:00</span>
    </div>
    <button class="rwd" data-icon="B" aria-label="rewind"></button>
    <button class="fwd" data-icon="F" aria-label="fast forward"></button>
  </div>
</div>
```
This div neatly contains the entire player for styling, has multiple sources to support different browsers, and a span in the controls to create a timer. The controls are each labeled with a class and an aria-label that indicates their nature, as well as given a data icon attribute to set the icon that will display. 
```css
.controls {
  visibility: hidden;
  opacity: 0.5;
  width: 400px;
  border-radius: 10px;
  position: absolute;
  bottom: 20px;
  left: 50%;
  margin-left: -200px;
  background-color: black;
  box-shadow: 3px 3px 5px black;
  transition: 1s all;
  display: flex;
}

.player:hover .controls, player:focus .controls {
  opacity: 1;
}
```
This first section of styling makes the controls switch opacity on mouse hover, sets the default to hidden (which can be changed by Javascript assuming it successfully implements), and adds some basic formatting for the controls as well. 
```css
@font-face {
   font-family: 'HeydingsControlsRegular';
   src: url('fonts/heydings_controls-webfont.eot');
   src: url('fonts/heydings_controls-webfont.eot?#iefix') format('embedded-opentype'),
        url('fonts/heydings_controls-webfont.woff') format('woff'),
        url('fonts/heydings_controls-webfont.ttf') format('truetype');
   font-weight: normal;
   font-style: normal;
}

button:before {
  font-family: HeydingsControlsRegular;
  font-size: 20px;
  position: relative;
  content: attr(data-icon);
  color: #aaa;
  text-shadow: 1px 1px 0px black;
}
```
The @font-face block brings in a custom set of controller icons for us to use. Then we set `content: attr(data-icon);` to make the icons correspond to the attribute based on the custom font-family. 
```css
.timer {
  line-height: 38px;
  font-size: 10px;
  font-family: monospace;
  text-shadow: 1px 1px 0px black;
  color: white;
  flex: 5;
  position: relative;
} 
  
.timer div {
  position: absolute;
  background-color: rgba(255,255,255,0.2);
  left: 0;
  top: 0;
  width: 0;
  height: 38px;
  z-index: 2;
} 
  
.timer span {
  position: absolute;
  z-index: 3;
  left: 19px;
} 
```
The timer is set to have a bar starting with a width of zero that JavaScript will widen as the timer increases, and a specific span selector that allows js to also increment the timer. 
  
The JavaScript recommended by the article, does several things:
  
- Establish variables that locate the key interactive nodes and selectors
- Listeners with functions that change the display of the buttons as well as ensure the desired effects are carried out. 
- Additional functionality to assure that the buttons interact correctly. 

These things combined together allow for a basic but cohesive video experience to be built into your site. 
  
[<<Return to Home](../README.md)