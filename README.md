eqHeights
=========

Responsive (or not) equal heights jQuery plugin

Example fiddle: http://jsfiddle.net/AbYcf/9/

To use:

Setup the html structure like:

<div class="boxes">
  <div class="box"></div>
  <div class="box"></div>
</div>

and in your JS call:

$(window).load($('.boxes').eqHeights('equilize')); //use window.load if you have images in your boxes.
$(window).resize(function () {
    $('.boxes').eqHeights(window.innerWidth > 320 ? 'equilize' : 'destroy');  
});