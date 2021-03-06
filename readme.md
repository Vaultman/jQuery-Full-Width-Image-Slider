# jQuery Full Width Image Slider

A jQuery full width slider designed to be as compatible and lightweight as possible. Minified (JS & CSS) it weighs in at just 3.3KB (~1.5KB gzipped).

Features:

* Total minified size - 3.3KB minified (~1.5KB gzipped)
* Fully Responsive
* Keeps images vertically centered
* Supports keyboard navigation
* Supports captions
* Resizes caption font for best viewing experience
* Multiple options
* Tested with:
	* Chrome 22 (OSX)
	* Safari 6 (OSX)
	* Firefox 16 (OSX)
	* iPad Safari (6.1)
	* iPhone Safari (6.1)
	* IE6 - works but with no navigation circles under slides & no transparency
	* IE7 - works but with no navigation circles under slides 
	* IE8-IE10 - works fine

#Important

If you require compatibility with IE8 and below then make sure you're using this IE detection method:

```html
<!--[if lt IE 7]> <html class="lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
<!--[if IE 7]> <html class="lt-ie9 lt-ie8"> <![endif]-->
<!--[if IE 8]> <html class="lt-ie9"> <![endif]-->
<!--[if IE 9 ]> <html class="ie9"> <![endif]-->
<!--[if gt IE 9]><!--> <html> <!--<![endif]-->
```


##Usage:



Include `slider.css` or `slider.min.css` and use the following html structure:

```html
<div class="full-width">
	<div class="inner">
		<div class="slide">
			<div>
				Lorem ipsum dolor sit amet, consectetur. <br>
				Curabitur molestie elit et ultricies vehicula.
			</div>
			<img src="http://lorempixel.com/1020/400/sports" width="1020" height="400">
		</div>
		<div class="slide">
			<!-- Caption can be omitted without any change in functionality -->
			<img src="http://lorempixel.com/1020/400/cats" width="1020" height="400">
		</div>
	</div>
	<div class="controls">
		<a href="#" class="left">&lt;</a>
		<a href="#" class="right">&gt;</a>
	</div>
	<div class="slide-nav"></div>
</div>
```

Then include `slider.js` or `slider.min.js` and initialise it using:

```javascript
$('.full-width').fullWidth();
```

The script automatically adds a CSS class to each slide in this format: `slide-1`, `slide-2`, `slide-3` etc. These allow you to specifically target slides if you need to add custom styles.

 
##Options:

```javascript
$(selector).fullWidth({
	maxHeight	:	450, // maximum height of slider, px
	minHeight	:	375, // minimum height of slider, px
	delay		:	5000, // delay between slides, ms
	transition	:	1000, // transition speed, ms
	maxFont		:	36, // maximum font size, px
	minFont		:	24 // minimum font size, px
});
```	
## License 

The MIT License (MIT)

Copyright (c) 2013 Joseph Bonham

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.