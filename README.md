# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- **Bonus**: Use the local JSON data to dynamically populate the content

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Json

### What I learned
This challenge taught me how to work with JSON data to dynamically update a webpage.
  Here's a exemple of code

```html
<script>
      const equipe =
      [
        {
          "category": "Reaction",
          "score": 80,
          "icon": "./assets/images/icon-reaction.svg"
        },
        {
          "category": "Memory",
          "score": 92,
          "icon": "./assets/images/icon-memory.svg"
        },
        {
          "category": "Verbal",
          "score": 61,
          "icon": "./assets/images/icon-verbal.svg"
        },
        {
          "category": "Visual",
          "score": 73,
          "icon": "./assets/images/icon-visual.svg"
        }
      ];
const conteneur = document.getElementById("RMV");

          equipe.forEach(membre => {
            const carte = document.createElement("div");
            carte.className = "carte";
            carte.innerHTML = `
          <div style="display: flex; align-items: center; gap: 10px;">
            <img src="${membre.icon}" alt="${membre.category}">
            <h5>${membre.category}</h5>
          </div>
          <p><span>${membre.score}</span> / 100</p>
        `;
            conteneur.appendChild(carte);
        });
</script>
```

### Continued development
I would like to learn more about using JSON in depth, and how it can be combined with JavaScript as well as other programming languages.

### Useful resources

## Author

- GitHub : [@MAXbcv](https://github.com/MAXbcv)
- Frontend Mentor : [@MAXbcv](https://www.frontendmentor.io/profile/MAXbcv)


## Acknowledgments
Thanks to the Frontend Mentor community for the inspiration and the many shared examples. This challenge helped me improve my web development skills
