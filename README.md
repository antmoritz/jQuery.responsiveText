# jQuery.responsiveText

A simple jQuery plugin to make a specific selector's or the whole page's text responsive.

## Examples
Making the whole page responsive (presuming that you're using `em` or `rem` units for other elements with a specified `font-size`):

	$("body").responsiveText();

Making all `<p>`aragraphs responsive:

	$("p").responsiveText();

## Configuration

There are three configuration options. `min`, `max` and `split` which can be passed into the plugin upon initialization. For example:

	$("body").responsiveText({
		min: 13,
		max: 20,
		split: 75
	});

### min (default: 12)

The smallest `font-size` acceptable.

### max (default 18)

Tha largest `font-size` acceptable.

### split (default 80)

What to divide `window.innerWidth` by to determine the `font-size`.

## Credits

Created by Karl Laurentius Roos. Inspired by Chris Coyier's article on [Viewport Sized Typography](http://css-tricks.com/viewport-sized-typography/).