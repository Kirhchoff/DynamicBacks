# DynamicBacks
Javascript library for handling dynamic background-images.

## Usage
1. Create instance of dynamic backgrounds handler for the object you want to animate:
  var dynaBack = createDynamicBack();
2. Initialize object with an array of background images, target object jQuery selector, duration of transition animation in seconds, background color, additional CSS style to append, using _initialize_ method:
  initialize(backgroundsArray, targetJQuerySelector, [duration, backgroundColor, additionalStyle]),
  
  for example:
  dynaBack.initialize(backgrounds, "#target", 0.4, "magenta", "background-position:center");
  
  Only the first two parameters are required. The rest has default values:
    - animation duration: 0.6,
    - background color: "white"
    - additional style: ""

  IMPORTANT: target element cannot have it's own background color specified in css. This will cover the animations. You can only specify the background color via aforementioned interface.

3. Trigger animation:
  dynaBack.nextBack();
  
  During the animation, trigger is disabled, so you cannot start another animation until the previous one finished.

## Example
https://codepen.io/Kirhchoff/full/aBgyae/
