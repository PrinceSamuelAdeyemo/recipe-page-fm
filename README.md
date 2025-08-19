# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### Screenshot

![](./result/Screenshot%202025-08-19%20at%2002-50-26%20Frontend%20Mentor%20Recipe%20page.png)


### Links

- Solution URL: (https://github.com/PrinceSamuelAdeyemo/recipe-page-fm)
- Live Site URL: (https://recipe-page-fm-xi.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Adjusting list elements appropriately using 'step-counter'
To see how you can add code snippets, see below:

```html
<div class="instructions">
  <h2 class="young-serif-regular">Instructions</h2>
  <ol>
    <li><span>Beat the eggs:</span> In a bowl, beat the eggs with a pinch of salt and pepper until they are well mixed. You can add a tablespoon of water or milk for a fluffier texture.</li>
    <li><span>Heat the pan:</span> Place a non-stick frying pan over medium heat and add butter or oil.</li>
    <li><span>Cook the omelette:</span> Once the butter is melted and bubbling, pour in the eggs. Tilt the pan to ensure the eggs evenly coat the surface.</li>
    <li><span>Add fillings (optional):</span> When the eggs begin to set at the edges but are still slightly runny in the middle, sprinkle your chosen fillings over one half of the omelette.</li>
    <li><span>Fold and serve:</span> As the omelette continues to cook, carefully lift one edge and fold it over the fillings. Let it cook for another minute, then slide it onto a plate.</li>
    <li><span>Enjoy:</span> Serve hot, with additional salt and pepper if needed.</li>
  </ol>
</div>
```
```css
.instructions ol {
  counter-reset: step-counter;
}

.instructions ol li {
  counter-increment: step-counter;
  margin-bottom: 12px;
  position: relative;
  padding-left: 1.5rem; 
}

.instructions ol li::before {
  content: counter(step-counter) ".";
  position: absolute;
  left: 0;
  font-weight: bold;
  color: hsl(30, 10%, 34%);
}
```

## Author

- Frontend Mentor - [@PrinceSamuelAdeyemo](https://www.frontendmentor.io/profile/PrinceSamuelAdeyemo)
- X (Twitter) - [@PrinceSamuel_A](https://x.com/PrinceSamuel_A)
- Linkedin - [samueladeyemo](https://www.linkedin.com/in/samueladeyemo/)