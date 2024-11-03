# p5.JS Group Fix
🔗 [Report](https://docs.google.com/document/d/197LLvZXauJRpocG0KSUylJNpRxrUTCShBL1Q2TjmeAY/edit?usp=sharing)

Website [Issue 516](https://github.com/processing/p5.js-website/issues/516) deals with the responsiveness of the p5.JS website, as certain text and/or classes are cut off when viewed on screens with smaller width. Nath and I's code for this fix can be found in our shared [forked repository](https://github.com/callybton/p5.js-website).

The changes were created in the styles/global.scss file’s .homepage-header-top selector. We adjusted the height and max-height properties and created a new rule for mobile screens using the existing $breakpoint-tablet. Previously, the height was set to a calculation that would not adapt to every screen type. Adjusting the default properties and using the custom variable –-spacing-sm in the “new” breakpoint fixes the responsiveness of the page while maintaining consistency with the global CSS style rules.

## How It Went
Beginning with the fix was fairly complicated at first. It took a while to find a good first issue we were interested in, properly building the project from source, and understanding all the files and organization. However, doing the fix itself was relatively simple: we were able to experiment with adding, deleting, and adjusting different properties, variables, and breakpoints to find the most appropriate way to make the page responsive.


