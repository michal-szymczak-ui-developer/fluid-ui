![Logo FLUID UI](http://fluid-ui.michalszymczak.com/logo-fluid-ui.svg=250x)

# Fluid UI - Modern CSS Starter

Fluid CSS Starter is CSS starter. The directories structure based on the Inverted Triangle CSS methodology. It uses CSS Variables, fluid spacers and typography.

# Quick Demo Preview

- [DEMO](http://fluid-ui.michalszymczak.com/)
- [Documentation](http://fluid-ui.michalszymczak.com/docs/)

## General directories structure

![Structure](http://fluid-ui.michalszymczak.com/fluid-ui-specificity.png)

```
./main.scss
./01-functions/
./02-mixins/
./03-settings/
./04-framework/
./05-base/
./06-layout/
./07-components/
./08-vendors/
./99-utilities/
```

Every subdirectory contains **\_index.scss** which imports all files from specific subdirectory.
The main scss **styles/main.scss** file merges all subdirectories.

## Tools

`./01-functions/`\
`./02-mixins/`

First two directories contain abstract tools - functions and mixins.
That is slightly different order than in standard Inverted Triangle CSS. Why? Sometimes we need a function or mixin to do some operations on variables eg. convert from pixels to rems.

## Settings

`./03-settings/`

Directory with global settings - design tokens / variables for spacings, colors, typography, icon font, components or vendor plugins.

## Framework

`./04-framework/`

If you App/Webpage uses external frameworks (eg. Bootstrap, PrimeNG etc) this is a place for:

- overwriting frameworks variables with our global variables,
- import additional frameworks files including variables, components, utilities etc.
  If you don't need external framework - feel free to remove this directory!

## Base

`./05-base/`

Base styling eg. body, typography, accessibility rules. If you dont use external framework this the place to include external CSS reset.

## Layout

`./06-layout/`

Layout directory defines main parts of layout like Header, Main, Sidebar or footer. They differ from components - they appear only once in a page / view.

## Components

`./07-components/`

Place to add components styling. From buttons, form controls, modals, card to more sophisticated ones.

## Vendor

`./08-vendor/`

Set vendors variables under the **style/03-settings** directory. But if we cannot style vendor plugin with variables add here additional styling by overwriting or extensioning vendor's CSS.

## Views

`./08-views/`

CSS for specific views like Promotion, Contact and so on.

## Utilities

`./08-utilities/`

Includes you own utilities. For start you have:

- colors (eg.: .text-primary, .bg-primary, .border-primary),
- texts (eg.: typography classes, truncations, line clamping)
- flow (helps keeping rhythm and flow - see Links section)
- grid (eg. )
- custom scrollbar,
- prose (for text static content),
- wrapper.

See index.html to se all utility classes. For you own classes don't hesitate to use **!important**.

## Links

- [Inverted Triangle CSS](https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/)
- [Utopia Fluid Responsive Design](https://utopia.fyi/)
- [Easy Fluid Typography](https://www.smashingmagazine.com/2022/10/fluid-typography-clamp-sass-functions/)
- [Cube CSS](https://cube.fyi)
- [Modern CSS Reset](https://github.com/hankchizljaw/modern-css-reset)
- [Flow](https://alistapart.com/article/axiomatic-css-and-lobotomized-owls/)
