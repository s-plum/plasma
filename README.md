# Solid

Solid is BuzzFeed's functional CSS framework builder and theming scaffolding. This library includes the standard BuzzFeed.com theme, and can be extended to suit other color palettes and layouts while maintaining consistent class names for rapid prototyping. For more details check out the [Solid Docs](https://solid.buzzfeed.com/).

## Using Solid

### Importing Solid

Solid can be as opinionated or as generic as you need for your purposes.

If you just want all of the default classes, breakpoints, and theme colors available in the BuzzFeed theme, all you need is:
```
/* main.scss */

@import "solid";
```

If you want to use all of the theme styles, but not all of the component classes, you can pick and choose. Be sure to include `solid-helpers` before any other imports, as that file contains all of the scaffolding variables and mixins:

```
/* main.scss */

/* I only need buttons and forms */
@import "solid-helpers";
@import "solid-utilities/buttons";
@import "solid-utilities/forms";
```

By default, both of these imports will give you classes for all of the BuzzFeed theme colors, and 4 different breakpoints. You can go a step further in your customization by creating your own theme file that overrides any of the defaults set in `solid-helpers/variables` to define exactly what breakpoints, sizes, and colors you need:
```
/* main.scss */

@import "solid-helpers/variables";
@import "solid-helpers/mixins";
@import "solid-helpers/theme";
@import "my-theme";
```

If you want to fully customize your theme and ditch all of that BuzzFeed red and blue, simply drop the solid theme and use your own:
```
/* main.scss */

@import "solid-helpers/variables";
@import "solid-helpers/mixins";
@import "my-theme";
```

The requirements for your own theme file are covered in the next section.

### Theming Solid

_Coming soon_

## Developing Solid
Any BuzzFeed employee can contribute to Solid. See [Contributing to Solid](https://github.com/buzzfeed/solid/blob/master/CONTRIBUTING.md).

## Todos
- [ ] Finish available theme params docs
- [ ] Test with CSS variables in theme file
- [ ] Check theme file - make sure all items are defined
- [ ] Bpager smoke test to make sure classes carry over
- [ ] Release as Solid 3.0-alpha
- [ ] Break things
