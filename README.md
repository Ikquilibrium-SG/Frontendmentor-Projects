# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements



### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow



### What I learned

I learned the following
- How to center a div for the umpteenth time
- How to center an image in a div but I had to make some little changes.
- How to place the content to be vertically aligned with centered image so that it appears in a consistent form from top to bottom. 

- I used opacity to design the horizontal line to make it appear as it is in the design image. This is the first time I'm using opacity.
- Used flexbox for the nft price, time left, the image and creator's name. 
- I found a way to align the ethereum image and the price together, did same with the clock image and the time left. This was something I thought of  when writing the css code for the project, I saw that the image was not on the same line as the words(This is probably due to the fact that I placed the images in the heading), I tried both padding and margin before going for margin. The margin top and bottom was given a negative value to achieve this. Anyways, I feel there will be a better way to get this done. The code is highlighted below

- I started this project on the 27th of Dec., 2021 and was true with almost everything on the third day. I had it tough to get the nft image to appear beneath the icon image with the icon image maintaining it white color. I applied opacity on hovering and I almost achieved the perfect result, the only problem was that the icon image color was affected also. I had to try different approach in the html file before arriving at the final result. I spent days trying different approach in the css file, googled a lot during this time and was frustrated. I posted the link that helped me to achieve the final result in the useful resources. You can check it out. 

```html
<h3 id="nft-price"><img class="item1-img" src="images/icon-ethereum.svg" alt="ethereum icon"> 0.041 ETH</h3>
<h3><img class="item1-img" src="images/icon-clock.svg" > 3 days left</h3>
```
```css
.item1-img {
    margin: -3.5px 0px;
    padding-right: 3px;
}
```

```html
<header class="img-container">
    <img class="img1" src="images/image-equilibrium.jpg" alt="equilibrium image NFT ">
    <img class="icon-img" src="images/icon-view.svg" alt="">
</header>
```
```css
.img-container {
    background-color: hsl(178, 100%, 50%);
    margin-top: 10px;
    width: 94%;
    border-radius: 10px;
    margin-left: 10px;
    position: relative;
}

.img1 {
    border-radius: 8px;
    margin-bottom: -4px;
    width: 100%;
}

.icon-img {
    position: absolute;
    left: 43%;
    top: 41%;
    width: 16%;
    height: auto;
    display: none;
}

.img-container:hover .icon-img {
    display: inline;
}

.img1:hover {
    opacity: 0.5;
    cursor: pointer;
}

```


### Continued development

I still feel there's a lot that I need to learn. 
I plan to learn either bootstrap or tailwind for css. I also want to learn to apply the HTML5 structure in my code.


### Useful resources

- [Changing image on hover](https://stackoverflow.com/questions/18813299/changing-image-on-hover-with-css-html) - This helped me to change the way I wanted the nft image and the hover image to appear. I thought that the method in the page appear more straight forward and clearer than what I intended to use. 

- [Change a css background image opacity] (https://www.digitalocean.com/community/tutorials/how-to-change-a-css-background-images-opacity), 
 [Change image on hover with css] (https://www.tutorialrepublic.com/faq/how-to-change-image-on-hover-with-css.php) - This provided the information I needed to get the result for the background image.

## Author

- Frontend Mentor - [@ikquilibriumSG](https://www.frontendmentor.io/profile/ikquilibrium)


## Acknowledgments

Well my thanks go to GOOGLE. Most of the challenges I encountered was solved by answers I got from google. I know that I need to improve the way I structure my questions.

