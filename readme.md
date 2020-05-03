# Gravity Forms Styles

This is a lean, modern, pretty, and flexible stylesheet for Gravity Forms.

Gravity Forms is awesome functionally, but the included styles are outdated and difficult to work with. This style package seeks to solve those issues by using:

- Minimal CSS selector nesting.
- Well organized SASS structure.
- SVG icon sprites (including SketchApp source files).
- Flex layout for variable fields.
- CSS Ready Classes included.
- Additional utility classes for hiding labels, styling submit buttons, etc.

## How to use.

All SASS files are partials. Variables use `!default`. Overrides are _easy_.

Import `_main.scss` into your primary SCSS theme file to automatically include all files. Before the import, set any of the theme variables that you want to override. In most situations, you should be able to customize the form just by overriding variables and never need to touch the source.

**NOTE:** The end goal is to have a system flexible enough that you really never need to touch source and just use overrides. You migh be able to just include this repo as a submodule in your theme and keep things easily up to date that way. _However_, this project is still in active development, so you should expect breaking changes for the time being. Factor that in.

Obviously, you could also just download the source and modify to your hearts content. If you do something broadly useful or more performant, please contribute it back to the main repo :)

### Utility classes.

A small assortment of classes to further style forms on a case-by-case basis. Utility classes should be added to a parent of your embeded form.

`.sv-form-hide-labels` hides all field labels. Best used with small lead capture style forms. Don't forget to use placeholders.

`.sv-form-button-m` and `.sv-form-button-l` make the submit button 50% wide and 100% wide respectively.

### Further considerations:

1. The default variable values (such as field height) have been optimized to play well in themes using Bootstrap.

2. Icons are base64 encoded and inlined in the stylesheets to prevent file-path complications when dropping this into your project. However, the assets are available in the repo so you can reference the images directly if you prefer to load them that way. It may situationally yield better page speed scores.

## Icons.

Icons are SVG sprites. There are two sprites:

1. Basic icons.
2. Credit card icons.

If you aren't using the default credit card field (and you probably shouldn't these days), set the `$gfs-use-credit-card-styles` to `false` to prevent compiling credit card field styles. The styles themselves don't necessarily take a log of space, but the encoded icons do, so this can noticeably reduce file size.

## WIP

This project powers a number of our own sites in production, but is also still in active development, so use at your own risk. If you find bugs or have feedback, please don't hesitate to get in touch. And most of all, if you have contributions, please make a pull request so we can review and add them in.

Enjoy!
