# Gravity Forms Styles

This is a lean, modern, pretty, and flexible stylesheet for Gravity Forms.

Gravity Forms is awesome functionally, but the included styles are outdated and difficult to work with. This style package seeks to solve those issues by using:

- Minimal CSS selector nesting.
- Well organized SASS structure.
- SVG icon sprites (including SketchApp source files).
- Flex layout for variable fields.
- CSS Ready Classes included.
- Additional utility classes for hiding labels, styling submit buttons, etc.

### How to use.

All SASS files are partials. Import `_main.scss` into your primary SCSS theme file to automatically include all files. For our sites, we do this by adding this repo as a GIT sub-module to our theme repos.

If you need to customize these styles, start by updating the `_variables.scss` file. A few tweaks to height, spacing, and color will be enough to fit into most style guides. That said, you could also fork this project and modify drastically for your own needs.

#### Further considerations:

1. These styles work particularly well when dropped into a theme that is using Bootstrap.

2. Icons are base64 encoded and inlined in the stylesheets to prevent file-path complications when dropping this into your project. However, the assets are included, so you can reference the images directly if you prefer to load them that way. It may situationally yield better page speed scores.

### Icons.

Icons are SVG sprites. There are two sprites:

1. Basic icons.
2. Credit card icons.

If you aren't using the default credit card field, commenting out the "CC Icons" section in `_variables.scss` and removing the import for `credit-card-field` in `_main.scss` wil reduce total file size by ~ 50k.

### WIP

This project powers a number of our own sites in production, but is also still in active development, so use at your own risk. If you find bugs or have feedback, please don't hesitate to get in touch. And most of all, if you have contributions, please make a pull request so we can review and add them in.

Enjoy!