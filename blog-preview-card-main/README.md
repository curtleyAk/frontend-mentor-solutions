# Frontend Mentor - QR code component solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![Screenshot of Project](<Screenshot 2025-05-04 at 08.25.55.png>)

### Links

- Solution URL: [Solution URL] - https://github.com/curtleyAk/frontend-mentor-solutions/tree/main/blog-preview-card-main
- Live Site URL: [Live URL] - https://curtleyak.github.io/frontend-mentor-solutions/blog-preview-card-main/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned

There isn't anything major I learnt, but there are some great tricks I picked up especially with responisveness. I do still struggle to import a for asset that was downloaded, so I used the Google Fonts URL instead. But I learnt using display=swap will make it load faster. also using font-size=clamp() to make the font size more scalable.

To see how you can add code snippets, see below:

```css
.preview__title h1 {
    /* Slace the font size as the view point width of the container becomes smaller */
    font-size: clamp(1.1rem, 1rem + 1.5vw, 1.5rem);
    font-weight: 800;
    margin-bottom: 12px;
}
.container {
    max-width: 300px;
    background: hsl(0, 0%, 100%);
    padding: 20px;
    border-radius: 20px;
    /* Set the margins to auto to center the container in the middle of the webpage */
    margin: auto;
}
.container img {
    /* Change the size of the image to be proportionate to it's parent container */
    max-width: 100%;
    height: auto;
    /* Change the display of the image to make sure all other content will fall below it */
    display: block;
    border-radius: 20px;
}
/* Because the margin in the container is set to auto, any other container will by default move to the bottom of the webpage */
.attribution {
    font-size: 11px; text-align: center;
    width: 100%;
    /* Prevent div from shrinking if content grows. */
    flex-shrink: 0; 
    margin-bottom: 10px;
}
```

### Continued development

I want to continue learning about CSS alignment like flexbox, grid and float in order to better display sections
in my websites.

### Useful resources

- [Example resource 1](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - This helped me scale font sizes to become smaller as the screen size becomes smaller.

## Author

- Website - [Curtley Kennedy](https://github.com/curtleyAk/)
- Frontend Mentor - [@curtleyAk](https://www.frontendmentor.io/profile/curtleyAk)
- Twitter - [@curtleyak](https://www.twitter.com/curtleyak)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

