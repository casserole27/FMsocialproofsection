# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](./images/Screenshot%202022-08-23%20at%2009-59-18%20Frontend%20Mentor%20Social%20proof%20section.png)


### Links

- Solution URL: https://casserole27.github.io/FMsocialproofsection/
- Live Site URL: https://www.clewisdev.com/FMsocialproofsection/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

SIMPLE two column layout using flex:
REMEMBER display: flex already flexes the layout, it's not necessary to add flex-direction: row

```css
.row {
  display: flex;
}

.column1 {
  width: 40%;
}

.column2 {
  width: 60%;
}
```


I learned more about backgrounds and background images in CSS.
This positions two SVGs in the top left and bottom right without repeat, and the percentages size them.
The max function on background-size helped me to size the SVGs for both mobile and desktop

```css
.body-wrapper {
background-image: url(/images/bg-pattern-top-desktop.svg), url(/images/bg-pattern-bottom-desktop.svg);
    background-position: top left, bottom right;
    background-repeat: no-repeat;
    background-size: max(50%, 400px), max(50%, 400px);
}


### Continued development

Inspirations from Kevin Powell's YouTube video:
The mobile and desktop designs worked seemed to work together seamlessly, whereas my typical designs are more clunky. I style one design a certain way, and then style the other a certain way with media queries, and it ends up being an almost separate style sheet. 
Reviewing grid and integrating it more, rather than reverting to flexbox always.
Learning to use transform: translate selector.
Learning to use flow-content inside of a HTML tag. This was a neat trick, are there others?
Implementing a better usage of variables, and overall more efficient CSS. 
Learning and using SASS. 

### Useful resources

- [Kevin Powell Frontend Mentor tutorial](https://www.youtube.com/watch?v=K27WULzr2P8&list=WL&index=1) - This is a complete walk-thu of this project done by Kevin Powell. It helped me to complete the project because I was stuck on the background SVGs, and it gave me a lot of ideas on how I can write more efficient CSS in the future.

## Author

- Website - [Cassie Lewis](https://www.clewisdev.com)
- Frontend Mentor - [@casserole27](https://www.frontendmentor.io/profile/casserole27)
- LinkedIn - (https://www.linkedin.com/in/clewisdev/)


## Acknowledgments

I'd like to acknowledge Kevin Powell's knowledge of CSS via his YouTube videos, and I'd like to check out more in the future to help refine my CSS skills.
