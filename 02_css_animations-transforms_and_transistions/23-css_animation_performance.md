## 2 Important Questions

1. What can be transitioned?
2. What should be transitioned?

1. What can be transitioned?
- lots of properties
- not all CSS props, but many
- but which ones will not affect website's performance?

2. What should be transitioned?
- 4 properties:
  1. transform: translate();
  2. transform: scale();
  3. transform: rotate();
  4. opacity
- can use others, but if working on enterprise, for mobile, or big app, should stick to these
- Why these properties?
- https://www.html5rocks.com/en/tutorials/speed/high-performance-animations/

Has to do with how browsers render webpages

- several stages in rendering webpage
  - e.g. calculating styles to apply to elements, determining where things should be
  - paint setup stage, paint stage: filling in pixels
  - finally: composite layers: transform and opacity
- this is a waterfall - to change properties defined at END means that browser doesn't have to re-do other calculations

This is NOT a hard rule, just keep it in mind!