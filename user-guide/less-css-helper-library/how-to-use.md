# less-css-helper-library

## How to use

Install the npm package or use the cdn option.

### Install [npm package](https://www.npmjs.com/package/@code-collabo/less-css-helper-library):

`npm i @code-collabo/less-css-helper-library`

Reference the library in your project with:

`node_modules/@code-collabo/less-css-helper-library/css/styles.css` - _For css project_.

`node_modules/@code-collabo/less-css-helper-library/less/styles.less` - _For less project_.

You can just _reference both_ in case you need to switch from `css` to `less` & vice versa. Make sure to add the reference\(s\) before that of your own css and/or less files.

If you are using less in an angular project for example, reference the one for less or both in the styles array in your angular.json file. You also need to import it at the top of your main .less file like so:

`@import 'node_modules/@code-collabo/less-css-helper-library/less/styles.less';`

### Using CDN:

For projects that don't use nodejs, add the css cdn as href value for your link tag in the .html file. Make sure to add this before the other link tags used to reference your own css styles.

`<link rel="stylesheet" href="https://code-collabo.github.io/less-css-helper-library/css/styles.css">`

### Class names:

From the class names, it's easy to tell what they do. See effect when added to an html element below:

* `.block` only sets display to block.
* `.grid` only sets display to grid. 
* `.flex` only sets display to flex.
* `.flex center` sets display to flex, justify-content & align-items are set to center. 
* `.flex-j-center` only sets display to flex & justify-content to center.
* `.flex-a-center` only sets display to flex & justify-content to center.
* `.flex-space-btw` sets display to flex & justify-content to space-between.
* Class names with _**suffix**_ `-auto` uses same styles as their look-alikes above, but make use of `margin: 0 auto;`. When applied on an element \(with width changed to less than 100%\), the element is horizontally centered. 
* `.b-container` uses same style as `block-auto`, but with width set & is _**responsive**_ already. To be used on the body element or html element\(s\) acting as outermost containers.
* _**Exception:**_ `x-auto` sets overflow to auto.
* `.grid-auto-1-auto-row` sets display to grid, grid-template-rows to `auto 1fr auto`, grid-template-columns to `1fr` & also sets the height of the element to 100%.
* `.img-wrapper` has same qualities of `.flex-center`, but with overflow set to hidden - to be used on the parent of an `img` element.
* `.img-wrapper-rounded` has same qualities of `.img-wrapper` but with border-radius set to 50% - to be used on the parent of an `img` element.
* `.img-default` is same as our [reset style](https://github.com/code-collabo/less-css-helper-library/blob/main/less/01-base/reset.less) for images. It sets an `img` element's max-width to 100% and height to auto. _**Note:**_ An `img` element inside a parent that uses `.img-wrapper` or `.img-wrapper-rounded` must be set to the reset style, therefore always add the `.img-default` class to such img element.
* `.error` and `.error-bold` are for text, while other color-related classes are for buttons.

You have total control over what the width of the element \(and margin in the case of `-auto`\) should be. More details & tutorial coming soon on this topic.

