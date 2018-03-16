## Changes

### Filesize

* I ran all the CSS through a minifier to reduce filesize.
* Ditto for the JS
* Compressed all the images to a much smaller filesize

### Convert

* I converted all the images to WEBP

### Critical CSS

* I used https://jonassebastianohlsson.com/criticalpathcssgenerator/ to check the critical css and pasted this inline into the index.html

### Fonts

* I added the font-display: swap;, so that the fallback font gets used first and then swapped to the webfont.

### Lazy Loading

* I added lazyloading to help on slower networks. Now images will only be loaded when it is in view.

## Before
![alt text](http://i.imgur.com/DxQtd8y.jpg "Logo Title Text 1")

## After
![alt text](http://i.imgur.com/d1kXaav.jpg "Logo Title Text 1")

## Where I messed up
![alt text](http://i.imgur.com/jIMEjvx.jpg "Logo Title Text 1")

If we look at these two images, you can see that the right one takes a full 3 seconds longer than the left one. Why is that you may wonder? One word. Extensions.

Extensions are amazing and lovely, but I forgot that some of them inject their own Javascript (and sometimes jQuery).

Testing without extensions saved me from a lot of frustrations 😩

