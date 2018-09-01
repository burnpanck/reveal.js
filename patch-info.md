# Information about the logical organisation of patches within branches

## Branch `burnpanck`
Super-patch of all following patches:
1. Branch `improve-fragments`
2. Branch `simplify-slide-API`
3. Branch `css-based-vertical-centering`

## Branch `improve-fragments`
Improves fragment API by adding an abstraction layer between fragments on the
DOM and how the code interacts with them. Patches the following files:
- `js/reveal.js`

## Branch `simplify-slide-API`
Improves slide API by adding explicit classes to the DOM elements that identify them
as slides or stacks. Added internal JS API to handle finding slides and stacks.
Patches the following files:
- `js/reveal.js`

## Branch `css-based-vertical-centering`
Adds a number of container divs around the slide contents such that each slide
lives on a fixed size canvas corresponding to the viewport size.
Therefore, one may now use CSS to position the slide content within the slide.
Unfortunately, this is a change that affects all themes.
Patches the following files:
- `js/reveal.js`
- `css/reveal.scss`
- `css/reveal.css` (generated file, derived from `css/reveal.scss`)
- `test/test-markdown-options.js`: The additional wrapper divs make the selector
  used to find the test target fail.
