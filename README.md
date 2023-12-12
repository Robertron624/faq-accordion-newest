# Frontend Mentor - FAQ accordion solution

This is a solution to the [FAQ accordion challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-wyfFdeBwBz). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- Hide/Show the answer to a question when the question is clicked
- Navigate the questions and hide/show answers using keyboard navigation alone
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://github.com/Robertron624/faq-accordion-newest)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I learned how to use the `details` and `summary` tags to create the accordions, a great addition to HTML that allow us to easily create accordions without using any javascript. I also learned how to use the `::after` pseudo element to replace the icons to the accordions.


The use of the `details` and `summary` tags
```html
<details class="question">
  <summary>
    <span> What is Frontend Mentor, and how will it help me? </span>
  </summary>
  <div class="content">
    <p>
      Frontend Mentor offers realistic coding challenges to help developers
      improve their frontend coding skills with projects in HTML, CSS, and
      JavaScript. It's suitable for all levels and ideal for portfolio building.
    </p>
  </div>
</details>
```

Handling the accordion icons
```css
details > summary::after {
  content: " ";
  background-image: url("./assets/images/icon-plus.svg");
  width: 30px;
  height: 30px;
  background-size: cover;
}

details[open] > summary::after {
  content: " ";
  background-image: url("./assets/images/icon-minus.svg");
  width: 30px;
  height: 30px;
}
```

### Continued development

I want to keep working on my CSS skills and learn more about CSS Grid and Flexbox. I also want to learn more about accessibility and how to make my sites more accessible, specifically for screen readers.

### Useful resources

- [Creating Accordions With Just HTML And CSS](https://blog.openreplay.com/creating-accordions-with-just-html-and-css/) - This helped me for the accordions, it uses semantic HTML and CSS only by using the `details` and `summary` tags. I really liked this pattern instead of using JS to toggle the accordions.

## Author

- Website - [Robert Ramirez](https://robert-ramirez.co)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Robertron624)
- Github - [@robertron624](https://github.com/Robertron624)
