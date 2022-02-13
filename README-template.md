# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

This is my solution to the 3-column preview card component. I added a few extra
features to make the desktop version a little more pleasant.

### Screenshot

![](./images/screenshot-desktop.png)
![](./images/screenshot-mobile.png)

### Links

- Solution URL: [GitHub](https://github.com/newbpydev/05-3-column-preview-card-component-main)
- Live Site URL: [Live Site](https://festive-roentgen-b5d430.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I have learned on this project that it is easy to get lost on which layout would
be best to use, I have tried both flexbox and grid to see which would be easier
to maintain later on. I have also tried the mobile-first approach and work my
way to the desktop version.

```css
  .wrapper {
    padding: 3.2rem 9.6rem;
    background-color: var(--prim-main-background-color);
    box-shadow: 0rem 0rem 3rem rgba(0, 0, 0, 0.2);
    position: relative;
  }

  .wrapper::before {
    position: absolute;
    content: "";
    height: 10%;
    width: 60%;
    background: linear-gradient(to left, rgba(170, 92, 219, 0), rgba(170, 92, 219, 0));
    transform: rotate(-3deg);
    left: 0rem;
    bottom: 2rem;
    z-index: -1;
    box-shadow: 3rem 3rem 3rem rgba(0, 0, 0, 0.5);
  }

  .wrapper::after {
    position: absolute;
    content: "";
    height: 10%;
    width: 60%;
    background: linear-gradient(to left, rgba(170, 92, 219, 0), rgba(170, 92, 219, 0));
    transform: rotate(3deg);
    right: 0rem;
    bottom: 2rem;
    z-index: -1;
    box-shadow: -3rem 3rem 3rem rgba(0, 0, 0, 0.5);
  }
```

### Continued development

For future development, I will continue to train using the flexbox and combine
it with the grid.

### Useful resources

- [MDN - CSS Filter](https://developer.mozilla.org/en-US/docs/Web/CSS/filter) - The filter CSS property applies graphical effects like blur or color shift to an element. Filters are commonly used to adjust the rendering of images, backgrounds, and borders.

## Author

- Website - [Juan Gomez](https://www.newbpydev.com)
- Frontend Mentor - [@newbpydev](https://www.frontendmentor.io/profile/newbpydev)
- Twitter - [@Newb_PyDev](https://twitter.com/Newb_PyDev)

## Acknowledgments

The code may not be perfect compared to my sensei @jonasschmedtman but I need
to thank him because he has shown me the ropes and now I am a confident web
designer.
