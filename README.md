# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://frontendmentor.io). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Design Screenshot](./Testimonial Grid Component.png) 


### Links

- Solution URL: [GitHub Repo](https://github.com/Agalya141/Testimonials_Grid_Section)
- Live Site URL: [Live Demo](https://agalya141.github.io/Testimonials_Grid_Section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS Custom Properties (Variables for HSL color schemes)
- CSS Grid (For asymmetric 2D multi-column layout)
- CSS Flexbox (For inner card card header structures and alignment)
- Responsive workflow with media queries
- Background image layer positioning

### What I learned

During this project, I significantly deepened my understanding of CSS Grid layouts and managing complex, multi-span grid tracks. Specifically, I practiced:

1. **Grid Track Structuring:** Learning how to config `grid-template-columns` on parent wrappers rather than child elements, using explicit tracks to manage multi-column structures.
2. **Asymmetric Spanning:** Mastering the use of `grid-column: span X` and `grid-row: span Y` to correctly stretch asymmetrical component card styles across varying axes.
3. **Fluid Layout Control:** Transitioning fixed components to a responsive state by using flexible fractional units (`1fr`) and `grid-template-rows: auto` to prevent structural text overflowing bugs.
4. **Layered Background Placement:** Fine-tuning decorative background assets (like quotation mark SVG files) using explicit background positional declarations so elements do not overlap border components.

```css
/* Example: Defining the asymmetric 4-column master container layout */
@media (min-width: 32rem) {
    .testimonial-container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: auto auto;
        gap: 1.5rem;
        max-width: 60rem;
        margin: 0 auto;
    }

    .first_card {
        grid-column: 1 / 3;
        grid-row: 1;
        background-image: url(bg-pattern-quotation.svg);
        background-repeat: no-repeat;
        background-position: top right 10%;
    }
}
```

## Continued development

In my upcoming layout developments, I intend to focus on:

- **BEM Naming Conventions:** Writing cleaner, more uniform HTML classes (Block-Element-Modifier) to replace arbitrary item class configurations.
- **Fluid Sizing Metrics:** Transitioning standard elements smoothly across screens without relying entirely on abrupt break-point adjustments.
- **Micro-interactions:** Integrating smooth transition hover configurations across individual block layout surfaces.

## Author

- GitHub - [@Agalya141](https://github.com/Agalya141)
- Frontend Mentor - [@Agalya141](https://www.frontendmentor.io/profile/Agalya141)
- LinkedIn - [Agalya M](https://www.linkedin.com/in/agalya6)
