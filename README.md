# Summary

This is an example project that has Bulma & SCSS installed ready to be themed.  It's meant to be a reference on how to configure Bulma with Angular using SCSS.

## Getting Started

To get hacking you need to do a few things.

Create a new Angular project if you don't have one.  `ng new some-angular-app`.

`cd` into your project's root `cd some-angular-app`

Install Bulma: `npm install bulma --save`

Copy this project's `src/assets/styles` folder into your project's assets folder `some-angular-app/src/assets`

Copy the contents of this project's `src/styles.scss` into your project's root stylesheet: `some-angular-app/src/styles.scss`

## Customizing

There are two files for initial and derived variables in `src/assets/styles/variables`.  They contain ALL of Bulma's initial, derived, and generic variables.
This is so you can see all of your customization options.  Change them as you see fit and they will be applied to the rest of Bulma.
Any that you don't plan on changing can be removed.

## Adding Custom Colors/Shades
Bulma comes with color helpers that let you do things like `html <p class="has-text-green">` and `html <p class="has-text-grey-darker">`.
If you want to be able to do stuff like `has-text-my-custom-color` or `has-text-grey-super-freakin-dark` do the following:
Declare a custom color: `$mintGreen`.
Add it to the `$custom-colors` or `$custom-shades` map in `derived.scss`.