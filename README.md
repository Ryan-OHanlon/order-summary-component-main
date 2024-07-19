# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover states for interactive elements

### Screenshot

![screenshot](./screenshot.jpeg)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/order-summary-component-using-css-flex-u85A40E6Fa](https://www.frontendmentor.io/solutions/order-summary-component-using-css-flex-u85A40E6Fa)
- Live Site URL: [https://ryan-ohanlon.github.io/order-summary-component-main/](https://ryan-ohanlon.github.io/order-summary-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

While this challenge was focused on applying hover states to <a> links. What I really learned was using the background-image attributes and properties to manipulate an image to stretch and create a wave effect as part of the background and use a background color to fill the blank space.

Using the background-repeat attribute and setting the property value to no-repeat prevented the image from repeating on both the x and y axis. Using the attribute background-size allowed me to set the width to cover the entire page and setting the height to 50% made the background image to only fill half of the web page while the background-color would be filled with the required background color.

```css
    background-image: url(./images/pattern-background-mobile.svg);
    background-repeat: no-repeat;
    background-size: 100% 50%;
    background-color: hsl(225, 100%, 94%);
```

The other thing I learned was using CSS flex to contain the musical note image, two lines of text, and a link. One of the difficult parts of designing a web page is manipulating multiple elements and have them be placed in a specific order when they are not going to be lined up on the y or x axis.

What I did was make a div element called .plan and used CSS Flexbox to contain the musical note image, the two <p> elements and the <a> element. Using justify-content attribute and setting the value to space-evenly between the elements. I then contained the two <p> elements in their own <div> container and use the built-in block rules so they would be as a single block instead by CSS Flex.

```css
.plan {
    background-color: hsl(225, 100%, 98%);
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    border-radius: 1em;
    margin: 1em;
    div{
        margin-right: 2em;
    }
    .annual {
        font-weight: 700;
        color: hsl(223, 47%, 23%);
    }
    .price {
        color: hsl(224, 23%, 55%)
    }
}
```

### Continued development

There is still a lot of CSS attributes that I'm not aware of and how to use them and their property values to be able to create these challenges in a time-efficient manner.

Each challenge has had me take the time to research certain attributes and ask questions on how to create the same effect.

### Useful resources

- [W3Schools](https://www.w3schools.com/cssref/css3_pr_background-size.php) - W3Schools is a good broad resource to understand the fundamentals of CSS attributes. However, you still will need to experiment and use each attribute yourself to really understand what each attribute does.

## Author

- Website - [Ryan O'Hanlon](https://ryan-ohanlon.github.io/)
- Frontend Mentor - [@Ryan-OHanlon](https://www.frontendmentor.io/profile/Ryan-OHanlon)
- Twitter - [@RyanROHanlon](https://x.com/RyanROHanlon)
