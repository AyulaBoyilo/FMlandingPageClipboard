# Frontend Mentor - Clipboard landing page solution

This is a solution to the [Clipboard landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/clipboard-landing-page-5cc9bccd6c4c91111378ecb9). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [How I did it](#how-i-did-it)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./design/desktop-design.jpg)

### Links

- Solution URL: [GitHub repository](https://github.com/AyulaBoyilo/FMlandingPageClipboard/)
- Live Site URL: [GitHub Pages](https://ayulaboyilo.github.io/FMlandingPageClipboard/)

## My process

### Built with

- Semantic HTML5 markup
- SCSS and CSS3
- CSS Flexbox

### How I did it

Used Sass mixin for button styles.

```scss
@mixin btn-main {
  display: inline-block;
  width: 100%;
  padding: 15px 0;
  margin-bottom: 20px;
  border-radius: 100px;
  transition: border-bottom 0.2s;
}

.btn {
  &-ios {
    @include btn-main;

    background-color: $strong-cyan;
    border-bottom: 4px inset darken($color: $strong-cyan, $amount: 7);

    &:visited {
      color: #fff;
    }

    &:hover {
      background-color: darken($color: $strong-cyan, $amount: 3);
      border-bottom: 4px inset darken($color: $strong-cyan, $amount: 10);
    }

    &:active {
      border-bottom: none;
    }
  }

  &-mac {
    @include btn-main;

    background-color: $light-blue;
    border-bottom: 4px inset darken($color: $light-blue, $amount: 7);

    &:visited {
      color: #fff;
    }

    &:hover {
      background-color: darken($color: $light-blue, $amount: 3);
      border-bottom: 4px inset darken($color: $light-blue, $amount: 10);
    }

    &:active {
      border-bottom: none;
    }
  }
}
```

### Useful resources

- [@mixin and @include](https://sass-lang.com/documentation/at-rules/mixin) - Sass Mixin Documentation page.

## Author

- Ayula Boyilo
