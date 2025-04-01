# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![](./images/Screenshot.png)

### Links

- Solution URL: [https://github.com/jamrollin/qr_code_component](https://github.com/jamrollin/qr_code_component)
- Live Site URL: [https://jamrollin.github.io/qr_code_component/](https://jamrollin.github.io/qr_code_component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties

### What I learned
#### text-align property 
  - applies to block containers. While, it doesn't apply directly to img element, putting it inside a block container such as div will center it. 

```html
 <div class="card">
    <img src="./images/image-qr-code.png" alt="frontendmentor.io QR code">
    <div class="content">
```
```css
* {
    margin: 0;
    padding: 0;
    font-family: Outfit;
    font-size: 15px;
    text-align: center;
}
```
#### span element
  - is an inline element so it won't respect vertical paddings or margins. In this project it's used as a container to line of texts for styling. For it to apply padding and margin property, it needs to be set as display: block. Used display: block instead of inline-block so the the text elements inside the span element are stacked on top of each other.

#### @font-face at-rule
  - to use custom font; can be loaded from a remote server or locally.
- It accepts property font-family for custom name. 
- font-weight property declares the range for text thickness. 
- font-display: swap > The swap period happens immediately after the block period, and during the swap period, fallback fonts are used until the custom font is loaded and swapped in.
- Use WOFF2 format as it is the newest and widely supported by browsers.
```css
@font-face {
    font-family: 'Outfit';
    font-weight: 400 700;
    font-display: swap;
    src: url('https://fonts.gstatic.com/s/outfit/v11/QGYvz_MVcBeNP4NJtEtq.woff2') format('woff2'); 
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

### Continued development

- [x] Using @font-face property
- Creating README.md document
- Hosting websites

### Useful resources

- [font best practices](https://web.dev/articles/font-best-practices)
- [font-display](https://savvy.co.il/en/blog/wordpress-speed/how-to-use-font-display-css)

## Author

