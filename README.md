# DynamicBacks
Javascript library for handling dynamic background-images.

## Usage
1. Create instance of dynamic backgrounds handler for the object you want to animate:
  var dynaBack = createDynamicBack();
2. Initialize object with an array of background images, target object jQuery selector, duration of transition animation in seconds, background color:
  dynaBack.initialize(backgrounds, "#target", 0.4, "magenta");
  
Default values:
  - animation duration: 0.6,
  - background color: "white"
  
IMPORTANT: target element cannot have it's own background color specified in css. This will cover the animations. You can only specify the background color via aforementioned interface.
3. Trigger animation:
  dynaBack.nextBack();

## Example
https://codepen.io/Kirhchoff/full/aBgyae/
