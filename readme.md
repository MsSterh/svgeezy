# SVGeezy
### A JavaScript plugin to handle your images in browsers that don't support SVGs

SVGeezy is in essence, a fallback plugin. It allows you to use SVGs for all your assets, giving you complete resolution independence.

It checks if the browser supports SVGs, if not, changes the _src_ of the image to a _.png_ instead (or whatever you pass in).

### Use

	svgeezy.init('nocheck', 'png');
	
The first parameter is a class to tell the code not to check. This may be because you have no fallbacks for certain SVGs. 

The second is a filetype, this can be anything you want, just make sure the file path resolves to an image. ie. _'/images/logo.svg'_, will be replaced with _'/images/logo.png'_.