# Frontend Mentor - Interactive rating component solution

This is a solution to the [Interactive rating component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-rating-component-koxpeBUmI). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Select and submit a number rating
- See the "Thank you" card state after submitting a rating

### Screenshot

![](./final_screenshots/desktop.png)


## My process

### Built with

- HTML
- CSS custom properties
- Flexbox
- jQuery
- Vanilla JS

### What I learned


```js //jquery to get the value of a radio button
  <script type="text/javascript">
      $('input[name="rate"]').on("click", function () {
        var rating = $('input[name="rate"]:checked').val();
        var ratingValue = document.getElementById("rating_value");
        ratingValue.innerHTML = rating;
      });
```
```js //hiding the first card after clicking on the button
  const submitButton = document.querySelector(".button");
      const card1 = document.getElementById("first");
      const card2 = document.getElementById("second");
      submitButton.addEventListener("click", onSubmit);

      function onSubmit() {
        card1.classList.add("hide");
        card2.classList.remove("hide");
```
```html /* adding jquery value to the sentence*/
<div class="feedback_mark">
          You selected&nbsp;
          <p id="rating_value">0</p>
          &nbsp;out of 5
        </div>
```

### Continued development

1. ccs position and cascade
2. vanilla js functions
3. jquery