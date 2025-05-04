# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

![Project Screenshot](<Screenshot 2025-05-04 at 13.10.57.png>)

### Links

- Solution URL: [Solution URL] - https://github.com/curtleyAk/frontend-mentor-solutions/tree/main/social-links-profile-main
- Live Site URL: [Live URL] - https://curtleyak.github.io/frontend-mentor-solutions/social-links-profile-main/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned

I learned our to import font style from local folder. Create custom cursor.

To see how you can add code snippets, see below:

```css
/* Import font style from local asset folder */
/* Define the Regular Font Weight */
@font-face {
    /* name of the font */
    font-family: 'Inter';
    src: url('../assets/fonts/static/Inter-Regular.ttf');
    /* Regular font weight */
    font-weight: 400;
    font-style: normal;
    /* Apply to have font load with better performance */
    font-display: swap;
}
#links .btn {
    /* Reset all default button styling  */
    all: unset;
}
#links .btn:hover {
    background: hsl(75, 94%, 57%);
    color: hsl(0, 0%, 20%);
    /* Add custom black cursor to the hover state */
    cursor: url('../assets/images/icons8-cursor-32.png'), pointer;
}

```

### Continued development

I want to continue learning about CSS alignment like flexbox, grid and float in order to better display sections
in my websites.


## Author

- Website - [Curtley Kennedy](https://github.com/curtleyAk/)
- Frontend Mentor - [@curtleyAk](https://www.frontendmentor.io/profile/curtleyAk)
- Twitter - [@curtleyak](https://www.twitter.com/curtleyak)