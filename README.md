# Plasma

Plasma is an experimental CSS framework framework. That's not a typo - it's a framework that allows you to build your own themed CSS framework with helper classes for colors, typography, spacing, layout, etc.

Plasma is based on the Solid framework, but updated with additional configurations to prevent generation of unused classes that can bloat CSS.

This is still a highly experimental and probably-not-quite-entirely-correct iteration, so feedback is highly encouraged!

## What happened to Solid?
Solid is BuzzFeed's functional CSS framework and styleguide, and is the default "theme" for Plasma. The style rules for Solid are defined in theme.scss. 

Not feeling Solid? Instead of doing this:
```
@import "solid-helpers"
```

Do this:
```
@import "solid-helpers/variables"
@import "solid-helpers/mixins"
@import "path/to/my/theme/variables"
```

For more details check out the [Solid Docs](https://solid.buzzfeed.com/).

## Developing Plasma
Any BuzzFeed employee can contribute to Plasma or Solid. See [Contributing to Solid](https://github.com/buzzfeed/solid/blob/master/CONTRIBUTING.md) and [Developing Solid](https://github.com/buzzfeed/solid/blob/master/DEVELOPING.md).

## Todos
- [ ] Better usage docs
- [ ] Check theme file - make sure all items are defined
- [ ] Bpager smoke test to make sure classes carry over
- [ ] Release as Solid 3.0-alpha
- [ ] Break things
