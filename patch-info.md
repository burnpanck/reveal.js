# Information about the logical organisation of patches within branches

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
