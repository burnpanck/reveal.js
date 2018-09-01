# Information about the logical organisation of patches within branches

## Branch `burnpanck`
Super-patch of all following patches:
1. Branch `improve-fragments`
2. Branch `simplify-slide-API`

## Branch `improve-fragments`
Improves fragment API by adding an abstraction layer between fragments on the
DOM and how the code interacts with them. Patches the following files:
- `js/reveal.js`

## Branch `simplify-slide-API`
Improves slide API by adding explicit classes to the DOM elements that identify them
as slides or stacks. Added internal JS API to handle finding slides and stacks.
Patches the following files:
- `js/reveal.js`
