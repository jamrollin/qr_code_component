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

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties

### What I learned
#### text-align selector 
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

- [@font-face best practices](https://web.dev/articles/font-best-practices), 
- (https://savvy.co.il/en/blog/wordpress-speed/how-to-use-font-display-css/)

## Author

