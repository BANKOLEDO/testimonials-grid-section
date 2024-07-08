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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

Desktop View

![](./images/Screenshot%20(149).png)

Mobile View 

![](./images/testimonial%20mobile%20view.png)

### Links

- Solution URL: [My Solution](https://github.com/BANKOLEDO/testimonials-grid-section)
- Live Site URL: [Page Preview](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

#### CSS Grid Layout

I used CSS Grid to create a flexible and responsive layout, ensuring the design adapts seamlessly across various screen sizes.

```css
.entire-page {
    display: grid;
    justify-items: center;
    align-items: center;
    row-gap: 2rem;
}

@media (min-width: 1240px) {
    .entire-page {
        grid-template-columns: repeat(4, auto);
        grid-template-rows: auto auto;
        column-gap: 2rem;
        row-gap: 2rem;
    }
}
```

#### Typography and Font Styling

I incorporated Google Fonts for a clean and modern look, applying different font weights and styles to create visual hierarchy and improve readability.

```css
@import url('https://fonts.googleapis.com/css2?family=Barlow+Semi+Condensed:wght@400;500;700&display=swap');

.entire-page {
    font-family: 'Barlow Semi Condensed', sans-serif;
}

.name {
    font-size: 1.2rem;
    font-weight: 500;
    color: var(--white);
}

.remark-highlight {
    font-size: 1.4rem;
    font-weight: 550;
    color: var(--white);
}
```

#### CSS Variables

I defined CSS variables to maintain a consistent color palette, streamlining the process of applying and managing colors across the entire stylesheet.

```css
:root {
    --moderate-violet: hsl(263, 55%, 52%);
    --very-dark-grayish-blue: hsl(217, 19%, 35%);
    --very-dark-blackish-blue: hsl(219, 29%, 14%);
    --white: hsl(0, 0%, 100%);
    --light-gray: hsl(0, 0%, 81%);
}

.first-container {
    background-color: var(--moderate-violet);
}

.second-container {
    background-color: var(--very-dark-grayish-blue);
}
```

#### Responsive Design

I utilized media queries to ensure the page is responsive and visually appealing on all devices.

```css
@media (min-width: 1240px) {
    .first-container {
        grid-column: 1 / 3;
        grid-row: 1 / 2;
        width: 100%;
        height: 100%;
    }

    .second-container {
        grid-column: 3 / 4;
        width: 100%;
        height: 100%;
    }

    .third-container {
        grid-column: 1 / 2;
        width: 100%;
        height: 100%;
    }

    .fourth-container {
        grid-row: 2 / 3;
        grid-column: 2 / 4;
        width: 100%;
        height: 100%;
    }

    .fifth-container {
        grid-column: 4 / 5;
        grid-row: 1 / 3;
        width: 20rem;
        height: 100%;
    }
}
```

#### Flexbox for Layout

I used Flexbox for the alignment and spacing of elements within the containers.

```css
.first-container {
    display: flex;
    flex-direction: column;
}

.top-block {
    display: flex;
    margin: 1.5rem 0 1rem 0;
    align-items: center;
}

.avatar {
    width: 3rem;
    height: 3rem;
    border: 4px solid hsl(263, 47%, 66%);
    border-radius: 50%;
    margin-left: 2rem;
}
```


## Author

- GitHub - [GitHub](https://github.com/BANKOLEDO)
- Frontend Mentor - [@BANKOLEDO](https://www.frontendmentor.io/profile/BANKOLEDO)
- Twitter - [@bankydavid12](https://www.twitter.com/bankydavid12)


