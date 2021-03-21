
## SCSS Helper

  

#### Full lightweight collection of SCSS Variables, Mixins and Placeholders


[![https://nodei.co/npm/@bz-projects/scss-helper.png?downloads=true&downloadRank=true&stars=true](https://nodei.co/npm/@bz-projects/scss-helper.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/@bz-projects/scss-helper)

  [![Build Status](https://travis-ci.com/bz-projects/scss-helper.svg?branch=master)](https://travis-ci.com/bz-projects/scss-helper) [![lerna](https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg)](https://lerna.js.org)

This is my development package for clean CSS Code. Here in this package you have a collection

of SASS Placeholders and Mixins and much more.

  

### Installation

  

Install Node.js and run this short command 

```
npm i @bz-projects/scss-helper
```

If you want to save to your development dependencies
```
npm i @bz-projects/scss-helper --save-dev
```

### Config

Import all SCSS Files into your custom scss file. 
```
@import '../node_modules/@bz-projects/scss-helper/style';
```
or 
```
@import '@bz-projects/scss-helper/style';
```

### Overvide

1. Create your SCSS File 
2. Import the style of the NPM Package. See Config
3. Override your variables before the @import line 

Example: 

```scss

// Colors 
$color-trans: transparent;
$color-primary: #005b96;
$color-secondary: #e6e6ea;

$color-white: #ffffff;
$color-light: #f4f4f8;

$color-black: #000000;
$color-dark: #2a363b;

$color-light-grey: #949a98;
$color-grey: #4a4e4d;

// Fonts 
$fonts-primary: 'Open Sans';
$fonts-secondary: 'Lato';

// Spacing 
$spacing-main: 40px;
$spacing-half: 20px;
$spacing-small: 10px;

// Import all SCSS functions
@import '@bz-projects/scss-helper/style';


// Write your SCSS Code
body {
    @extend %bg-primary;
}

```