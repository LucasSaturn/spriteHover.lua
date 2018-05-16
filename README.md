# spriteHover.lua
Simple library for testing mouse over in Love2D. It takes into account, the sprite and it's alpha channel. Simply set the sprite information as parameters (detailed in the README file), and it will return a true or false value. 

### USAGE

To use spriteHover.lua, you must do the following:

*	declare an image data variable, using `love.image.newImageData()`
*	declare the scale of the sprite onscreen
*	declare the x and y co-ordinates of the sprite onscreen


Since this script is extremely basic, you are not able to use rotation on your sprites. There may be a future update that allows this, but for now, no rotation is allowed.

### Function: testMouseOver()
Parameters:

*	spriteX, X position of the sprite on screen
*	spriteY, Y position of the sprite on screen
*	spriteImageData, contains the pixel data, declared by `love.image.newImageData()
*	scaleX, X scale of the sprite on screen
*	scaleY, Y scale of the sprite on screen

### Actually implementing it within a program

You must add this script as a reference, and then place the test function in your code.

```require "location/spriteHover"```

The easiest way to handle other objects overlapping, is to test within the `love.draw()` function, and test each object. Then, the variable will be overwritten with a different object if the one you are testing for has a different sprite overlapping.
