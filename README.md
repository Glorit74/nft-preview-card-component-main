# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

### Screenshot

![](images/screenshot.jpg)

### Links

- Solution URL: [https://github.com/Glorit74/nft-preview-card-component-main](https://github.com/Glorit74/nft-preview-card-component-main)
- Live Site URL: [https://glorit74.github.io/nft-preview-card-component-main/](https://glorit74.github.io/nft-preview-card-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Hover

### What I learned

I couldn't think of a better one, although there is definitely a more elegant solution.

```html
<div class="equilibrium_img"><a href="#"></a></div>
```

```css
.equilibrium_img {
  height: calc(320px - 2.5em);
  overflow: hidden;
  border-radius: 0.75rem;
  background-image: url(/images/image-equilibrium.jpg);
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}

.equilibrium_img::after {
  content: "";
  display: block;
  height: calc(320px - 2.5em);
  z-index: 10;
  border-radius: 0.75em;
  opacity: 0.2;
  cursor: pointer;
}

.equilibrium_img:hover::after {
  background-color: var(--clr-accent);
}
```

## Author

- Frontend Mentor - [@Glorit74](https://www.frontendmentor.io/profile/Glorit74)

## Acknowledgments

Thanks to my school, **Codecool**!
