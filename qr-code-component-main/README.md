# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](./screenshot.jpg)

![alt text](<Screenshot 2025-05-01 at 17.17.11.png>)

### Links

- Solution URL: [Solution URL] - https://github.com/curtleyAk/frontend-mentor-solutions/tree/main/blog-preview-card-main
- Live Site URL: [Live URL] - https://curtleyak.github.io/frontend-mentor-solutions/blog-preview-card-main/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned

I learnt a bit about flexbox, still have a long way to go, but at least it makes sense

To see how you can add code snippets, see below:

```css
body {
    display: flex;
    /* Stack the container vertically */
    flex-direction: column;
    min-height: 100vh; /* make sure the body is displayed over the entire webpage */
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
    width: 100%;
    /* Prevent div from shrinking if content grows. */
    flex-shrink: 0;
    margin-bottom: 10px;
}
```

### Continued development

I want to continue learning about CSS alignment like flexbox, grid and float in order to better display sections
in my websites.


## Author

- Website - [Curtley Kennedy](https://github.com/curtleyAk/)
- Frontend Mentor - [@curtleyAk](https://www.frontendmentor.io/profile/curtleyAk)
- Twitter - [@curtleyak](https://www.twitter.com/curtleyak)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

