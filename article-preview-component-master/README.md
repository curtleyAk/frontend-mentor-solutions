# Frontend Mentor - Article preview component solution

This is a solution to the [Article preview component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/article-preview-component-dYBN_pYFT). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See the social media share links when they click the share icon

### Screenshot

![Mobile state](./assets/Screenshots/Screenshot%202025-09-27%20at%2015.17.45.png)
![Mobile active state](./assets/Screenshots/Screenshot%202025-09-27%20at%2015.17.54.png)
![Desktop state](./assets/Screenshots/Screenshot%202025-09-27%20at%2015.23.06.png)
![Desktop active state](./assets/Screenshots/Screenshot%202025-09-27%20at%2015.22.01.png)

### Links

- Solution URL: https://github.com/curtleyAk/frontend-mentor-solutions/tree/main/article-preview-component-master
- Live Site URL: https://curtleyak.github.io/frontend-mentor-solutions/frontend-mentor-solutions/tree/main/article-preview-component-master

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop-first workflow
- Vanilla JavaScript for DOM manipulation

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

This project was a fantastic exercise in managing complex UI states that change with screen size. My biggest takeaway was learning how to handle a single user action (a button click) that results in two completely different visual outcomes for desktop and mobile.

One of the most challenging parts was positioning the desktop share tooltip. I learned how to use a combination of position: relative on the parent container and position: absolute on the child to precisely place the tooltip. Creating the small triangle underneath it with a pseudo-element was also a great trick.

To see how you can add code snippets, see below:

```css
.author {
  display: flex;
  justify-content: space-between;
  position: relative;
}
.author.active .share-tooltip {
  display: flex;
  position: absolute; /* Lifts the tooltip out of the normal document flow. */
  z-index: 2; /* Ensures the tooltip appears on top of other content. */
  /* These values are fine-tuned to position the tooltip above the share button. */
  bottom: 170%;
}
```

The most significant "aha!" moment came when trying to style the mobile active state. My initial attempts were messy because I was fighting against the position: absolute from the desktop styles. I learned that I could "reset" an element's positioning inside a media query to make it behave like a normal element again. This simplified the CSS dramatically.

```js
function sharePopUp() {
  document.querySelector(".author").classList.toggle("active");
}
```

```css
/* Overrides the desktop tooltip styles for the mobile view. */
.author.active .share-tooltip {
  position: static; /* CRITICAL: Resets the positioning to flow normally. */
  background-color: transparent; /* Parent now has the background color. */
  padding: 0;
  box-shadow: none;
  justify-content: flex-start;
  order: -1; /* Flexbox trick to make the share info appear before the button. */
}
```

### Continued development

For future projects, I want to focus on a mobile-first workflow. I built this component desktop-first, and I'm curious to see how starting with the mobile layout would change my process and CSS structure.

I also want to dive deeper into accessibility (a11y). For this component, I could explore using ARIA attributes (like aria-expanded) on the share button to let screen reader users know that the button controls a collapsible element.

### Useful resources

- [Example resource 1](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This is my go-to guide for anything related to Flexbox. It's incredibly comprehensive.
- [Example resource 2](https://developer.mozilla.org/en-US/docs/Web/CSS/position) - his helped me finally understand the relative/absolute positioning relationship that was crucial for the desktop tooltip.
- [Example resource 3](https://css-tricks.com/the-shapes-of-css/) - A fantastic article that shows how to create different shapes, like the triangle for the tooltip, using pure CSS.

## Author

- Website - [Curtley Kennedy](https://github.com/curtleyAk/)
- Frontend Mentor - [@curtleyAk](https://www.frontendmentor.io/profile/curtleyAk)
- Twitter - [@curtleyak](https://www.twitter.com/curtleyak)
