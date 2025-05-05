# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

![Project Solution Screenshot](<../social-links-profile-main/Screenshot 2025-05-04 at 13.10.57.png>)

### Links

- Solution URL: [Solution URL] - https://github.com/curtleyAk/frontend-mentor-solutions/tree/main/recipe-page-main
- Live Site URL: [Live URL] - https://curtleyak.github.io/frontend-mentor-solutions/recipe-page-main/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I was able to do a lot better with positioning thit time. I learnt a lot about how to target particular elements using ::marker. I also did some light scanning through aespect-ratios's, I want know a bit more about those. I also started using margin-block-end instead of margin-bottom, still wrapping my head around the concept to see if there's any differance. Also border-collapse, this is to merge two elements' borders to make it more cleaner and uniform.
I liked using span in HTML to target text in order to apply a style, it's not a foreign concept, but haven't used it in a while.

To see how you can add code snippets, see below:

```html
<aside class="preparation__info">
      <h3>Preparation time</h3>
      <ul>
        <li><span>Total:</span> Approximately 10 minutes</li>
        <li><span>Preparation:</span> 5 minutes</li>
        <li><span>Cooking:</span> 5 minutes</li>
      </ul>
    </aside>
```
```css
header img {
    width: 100%;
    /* adjust the Images dimensions to maintain the specified width-to-height ratio within the container*/
    aspect-ratio: auto;
    border-radius: 0.75rem;
    margin-block-end: 2.5rem;
}
/* li::maker allows you to tarket the list marker and change its sizing and colour */
.preparation__info li::marker, #ingrediants li::marker {
    font-size: 0.8rem;
    color: hsl(332, 51%, 32%);
}
hr {
    margin-block: 2rem;
    /* Change the colour and size of the horizontal line rule */
    border-top: 1px solid hsl(30, 18%, 87%);
}
/* Targets the list numbers */
#instructions li::marker {
    font-weight: 700;
    color: hsl(332, 51%, 32%);
}
#nutritional__info table {
    width: 100%;
    border-collapse: collapse; /* Makes borders cleaner */
}
```

### Continued development

I want to continue learning about CSS alignment like flexbox, grid and float in order to better display sections in my websites.

### Useful resources

- [Example resource 1](https://developer.mozilla.org/en-US/docs/Web/CSS/aspect-ratio) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://developer.mozilla.org/en-US/docs/Web/CSS/::marker) - The ::marker CSS pseudo-element selects the marker box of a list item, which typically contains a bullet or number. 
- [Example resource 3](https://developer.mozilla.org/en-US/docs/Web/CSS/border-collapse) - Adjacent cells have shared borders (the collapsed-border table rendering model).


## Author

- Website - [Curtley Kennedy](https://github.com/curtleyAk/)
- Frontend Mentor - [@curtleyAk](https://www.frontendmentor.io/profile/curtleyAk)
- Twitter - [@curtleyak](https://www.twitter.com/curtleyak)
