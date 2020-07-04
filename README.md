# Stylesheet for FrontierJS

I want a methodology for styling

A way to think about it so I don't have to think about it

Currently at 4kb gzipped, 24kb minified

3 Types of Elements

- Containers // display: block
- Content Blocks // display: block
- Text Objects //display: inline-block

## Settings: preprocessor variables, colors, global settings

@import 's-color-palette'; // Need to build out refer others

@import 's-variables';

@import 's-breakpoints';

## Generic/Elements: element selectors, CMS-generated content

@import 'e-mixins'; //Don't need to touch unless adding mixin

@import 'e-reset'; //Don't touch, just default resetCSS

@import 'e-base'; // Fine tune this one

//Master Container Layout
maybe a default on main?

## Utilities: specific helper classes, overrides

@import 'u-containers';

// Aside? - what if asides have display none at certian media queries

//Border radius defaults

@import 'u-text';

// do we want a text component like ply/text?

// default word-wrap

// hr

// br

@import 'u-generic';

//Display

//Overflow

//Position

//Opacity

## Components: separately styled components (buttons, form inputs, toolbars...)

What are the Key components

@import 'c-form-input'; (Selects and Checkboxes)

@import 'c-button';

- Lists
- Tables
- Links
- Modal

What about true components like card or slider?
