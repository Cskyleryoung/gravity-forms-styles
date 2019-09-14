# Gravity Forms Styles

This is a lean, modern, pretty, and flexible stylesheet for Gravity Forms.

Gravity Forms is awesome, but the basic styles are outdated, bulky, and way over nested, making them difficult to override. It's time for an update.

Although this solution can be used as is, it's also meant to be used as a starting point for customization.

## What's here.

- Minimal CSS selector nesting.
- Well organized SASS structure.
- SVG icon sprites (including SketchApp source files).
- Flex layout for variable fields.
- CSS Ready Classes included.
- Additional utility classes for hiding labels, styling submit buttons, etc.

## How to use.

All SASS files are partials, entended to be imported into your theme or child theme stylesheet via a `style.scss` file. Import `_main.scss` and you are ready to go.

For customization, start by updating the `_variables.scss` file. A few tweaks to height, spacing, and color will be enough to fit into most style guides.

### Further considerations:

1. These styles work particularly well when dropped into a theme that is using Bootstrap.

2. Icons are base64 encoded and inlined in the stylesheets to prevent file-path complications when dropping this into your project. However, the assets are included, so you can reference the images directly if you prefer to load them that way. It may situationally yield better page speed scores.

## Icons.

Icons are SVG sprites. There are two sprites:

1. Basic icons.
2. Credit card icons.

If you aren't using the default credit card field, commenting out the "CC Icons" section in `_variables.scss` and removing the import for `credit-card-field` in `_main.scss` wil reduce total file size by ~ 50k.

## WIP

Not every style for every field is included, however this project is behind a large number of production sites and is in active development. We are open to suggestions, feedback, and espeically contributions. If you have code to contribute, please submit a pull request.

Thanks!



