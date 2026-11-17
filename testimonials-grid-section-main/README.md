# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

Assignment requirements covered:

- A container `<div>` holding the whole testimonials section, with each testimonial in its own `<div>` (photo, name, title and feedback text)
- `display: grid` on the container, with `grid-template-columns`, `grid-template-rows`, `grid-template-areas` and `gap`
- Testimonials of different sizes, spanning multiple columns/rows
- Media queries: 1 column on mobile, 4 columns on desktop
- Styling from the style guide, with `padding`, `border-radius` and `box-shadow`
- Reusable classes for the card colour themes

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid (with `grid-template-areas`)
- Mobile-first workflow
- Media queries

### What I learned

I learned how `grid-template-areas` makes it easy to see a layout directly in the code, and how to change that layout at a breakpoint without touching the HTML:

```css
.testimonials {
  grid-template-areas:
    "daniel"
    "jonathan"
    "jeanette"
    "patrick"
    "kira";
}

@media (min-width: 62rem) {
  .testimonials {
    grid-template-columns: repeat(4, 1fr);
    grid-template-areas:
      "daniel   daniel   jonathan kira"
      "jeanette patrick  patrick  kira";
  }
}
```

I also used reusable modifier classes (`.testimonial--purple`, `.testimonial--white`, etc.) so the colours are separated from the layout.

### Continued development

- Testing more screen sizes between 320px and large desktops
- Improving accessibility, such as checking colour contrast on the semi-transparent text

### AI Collaboration

I used Claude to generate the HTML and CSS from the assignment requirements and the design preview. I reviewed the code afterwards and checked it against the design.

## Author

- Name - [Add your name here]
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
