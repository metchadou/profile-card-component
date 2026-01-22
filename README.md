# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![./screenshot.png](./screenshot.png)

### Links

- Solution URL: [https://github.com/metchadou/profile-card-component](https://github.com/metchadou/profile-card-component)
- Live Site URL: [https://metchadou.github.io/profile-card-component](https://metchadou.github.io/profile-card-component)

## My process

### Built with

- HTML5
- CSS

### What I learned

This project helped me better understand how the pseudo-elements ::before and ::after work. My main challenge was positioning the two background images. A couple of resources listed in the next section helped me with this.

Here is how I did it:

```css
body {
    /*Other code here...*/
    position: relative;
}


body::before, body::after {
    content: '';
    position: absolute;
    width: 50vw;
    background-repeat: no-repeat;
    background-size: 130%;
    z-index: -1;
}

body::before {
    left: 0;
    top: 0;
    height: 70vh;
    background-image: url('images/bg-pattern-top.svg');
    background-position: bottom right;
}

body::after {
    bottom: 0;
    right: 0;
    height: 50vh;
    background-image: url('images/bg-pattern-bottom.svg');
    background-position: top left;
}
```

### Useful resources

- [https://discord.com/channels/824970620529279006/1444601277571923998](https://discord.com/channels/824970620529279006/1444601277571923998) - This discussion pointed me in the right direction when trying to position the background images.
- [https://youtu.be/dIUOWdwwZBw](https://youtu.be/dIUOWdwwZBw) - This is a short video that helped me understand the pseudo elements ::before and ::after.

## Author

- Frontend Mentor - [@metchadou](https://www.frontendmentor.io/profile/metchadou)