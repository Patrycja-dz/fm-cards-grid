# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size.
- See hover states for interactive elements.

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (Variables)
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project was a great opportunity to practice responsive design using CSS Grid and Flexbox. I focused on creating a clean HTML structure and maintainable CSS.

Here's a snippet of the HTML structure for the cards:

```html
<div class="card__wrapper">
  <div class="card card-cyan">
    <div>
      <h3 class="text-preset-3">Supervisor</h3>
      <p class="text-preset-5">
        Monitors activity to identify project roadblocks
      </p>
    </div>
    <img src="./images/icon-supervisor.svg" alt="" />
  </div>
  <!-- ... other cards ... -->
</div>
```

And an example of using CSS custom properties for theming:

```css
:root {
  --red: hsl(0, 78%, 62%);
  --cyan: hsl(180, 62%, 55%);
  --orange: hsl(34, 97%, 64%);
  --blue: hsl(212, 86%, 64%);

  --very-dark-blue: hsl(234, 12%, 34%);
  --grayish-blue: hsl(212, 6%, 44%);
  --very-light-gray: hsl(0, 0%, 98%);
  --white: hsl(0, 0%, 100%);

  --font-family-default: "Poppins", sans-serif;
  /* ... other variables ... */
}

.card {
  background-color: var(--white);
  border-radius: var(--space-100);
  /* ... other styles ... */
  border-top-style: solid;
  color: var(--grayish-blue);
}

.card-cyan {
  border-top-color: var(--cyan);
}
.card-red {
  border-top-color: var(--red);
}
```

I also implemented a simple hover animation for the card icons:

```css
.card img:hover {
  animation: tilt-shaking 0.25s infinite;
}

@keyframes tilt-shaking {
  0% {
    transform: rotate(0deg);
  }
  25% {
    transform: rotate(5deg);
  }
  50% {
    transform: rotate(0deg);
  }
  75% {
    transform: rotate(-5deg);
  }
  100% {
    transform: rotate(0deg);
  }
}
```

### Continued development

I plan to continue focusing on advanced CSS Grid layouts and explore more complex animations and transitions in future projects. I also want to get more practice with JavaScript to add more interactivity.

## Author

- [Frontend Mentor Account](https://www.frontendmentor.io/profile/Patrycja-dz)

## Acknowledgments

Thanks to Frontend Mentor for providing this challenge. (Add any other acknowledgments here)
