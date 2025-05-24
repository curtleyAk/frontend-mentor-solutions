# Frontend Mentor - Four card feature section solution

his is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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


## Overview

### Screenshot

![Project Solution Screenshot](<images/Screenshot 2025-05-24 at 13.08.39.png>)

### Links

- Solution URL: [Solution URL] - https://github.com/curtleyAk/frontend-mentor-solutions/tree/main/four-card-feature-section-master
- Live Site URL: [Live URL] - https://curtleyak.github.io/frontend-mentor-solutions/four-card-feature-section-master

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Grid

### What I learned

I was able to do a lot better with positioning thit time. I created a reset css stylesheet which I will be using in every project to prevent default styling from affecting my styles. I used the pseudo selctor, nth-child to apply styling to individual containers.

To see how you can add code snippets, see below:

```css
* Apply a natural box layout model to all elements and pseudo-elements */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove default margin and padding from an initial set of elements */
body, h1, h2, h3, h4, h5, h6, p,
ul, ol, li, figure, figcaption, blockquote, dl, dd {
  margin: 0;
  padding: 0; /* Some prefer to only reset margin and keep padding where it might be useful, like on lists */
}

/* Set core root defaults */
html {
  line-height: 1.5; /* A good default for readability */
  -webkit-font-smoothing: antialiased; /* Improve font rendering */
  -moz-osx-font-smoothing: grayscale; /* Improve font rendering */
}

/* Remove list styles on ul, ol elements with a list role, which suggests they are for navigation/layout */
ul[role='list'],
ol[role='list'] {
  list-style: none;
}

/* Make images easier to work with */
img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}

/* Inherit fonts for inputs and buttons */
input, button, textarea, select {
  font: inherit;
}

/* Remove all animations and transitions for people that prefer not to see them */
@media (prefers-reduced-motion: reduce) {
  html:focus-within {
   scroll-behavior: auto;
  }
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
.card:nth-child(1){
    border-top: hsl(180, 62%, 55%) 0.25rem solid;
}
.card:nth-child(2){
    border-top: hsl(0, 78%, 62%) 0.25rem solid;
}
.card:nth-child(3){
    border-top: hsl(34, 97%, 64%) 0.25rem solid;
}
.card:nth-child(4){
    border-top: hsl(212, 86%, 64%) 0.25rem solid;
}
```

### Continued development

I want to continue learning about CSS alignment like flexbox, grid and float in order to better display sections in my websites.

### Useful resources

- [Example resource 1](https://css-tricks.com/snippets/css/complete-guide-grid/) - A guide to CSS grid, focusing on all the settings both for the grid parent container and the grid child elements.


## Author

- Website - [Curtley Kennedy](https://github.com/curtleyAk/)
- Frontend Mentor - [@curtleyAk](https://www.frontendmentor.io/profile/curtleyAk)
- Twitter - [@curtleyak](https://www.twitter.com/curtleyak)
