 Frontend Mentor - QR code component solution

This is my solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

This project was built as part of my practice in **HTML and CSS**, with a focus on creating a clean, responsive QR code component and understanding CSS Flexbox, dimensions, spacing, typography, and the CSS box model.

Table of contents

  * [Links](#links)
* [My process](#my-process)

  * [Built with](#built-with)
  * [What I learned](#what-i-learned)
  * [Continued development](#continued-development)
  * [Useful resources](#useful-resources)
  * [AI Collaboration](#ai-collaboration)
* [Author](#author)
* [Acknowledgments](#acknowledgments)

 Links

* Solution URL: [View my solution on Frontend Mentor](https://www.frontendmentor.io/)
* Live Site URL: [View the live website](https://your-live-site-url.com)

 My process

Built with

* Semantic HTML5 markup
* CSS
* CSS Flexbox
* Responsive image sizing
* CSS `text-align`
* CSS `border-radius`
* CSS box model
* Google Fonts

What I learned

This project helped me strengthen my understanding of HTML and CSS, particularly how elements are positioned and sized within a page.

 1. Using Flexbox to center the component

I used Flexbox on the `body` to center the QR code component horizontally and vertically.

```css
body {
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
```

I learned that `justify-content` and `align-items` work according to the direction of the flex container.

Since I used:

```css
flex-direction: column;
```

the elements are arranged vertically, allowing the QR card and footer to appear one below the other.

 2. Understanding component dimensions

I gave the QR card a width of `320px` and added `16px` of padding.

```css
.outer {
  width: 320px;
  padding: 16px;
  border-radius: 15px;
}
```

I learned that dimensions are affected by the CSS box model. Padding adds space inside an element and can therefore affect its total size depending on the value of `box-sizing`.

The QR image uses:

```css
img {
  width: 100%;
  display: block;
}
```

This allows the image to take the full available width of its container rather than using a fixed image width.

 3. Why I didn't use a media query

I initially considered using a media query to change the size of the card for smaller screens.

However, I decided not to use one because the component is relatively simple and the layout can work without introducing a breakpoint.

The card has a fixed width of `320px`, while the image uses `width: 100%` to fit the available space. Flexbox is also used to keep the component centered.

For a small component like this, adding a media query just to change the card dimensions would add unnecessary CSS if the existing layout already works across the required viewport sizes.

This helped me understand that **responsive design does not always require media queries**. A layout can sometimes remain responsive through flexible sizing, appropriate dimensions, and Flexbox.

 4. Centering text

I used `text-align: center` to center the text within the card.

```css
.text {
  text-align: center;
}
```

This helped me understand the difference between positioning an element itself and aligning the content inside that element.

 5. Understanding spacing

I experimented with `padding` and `margin` to create space between the QR image, text, card, and footer.

For example:

```css
.outer {
  padding: 16px;
}

.text {
  margin: 25px;
}
```

This helped me understand how padding creates space **inside** an element, while margin creates space **outside** an element.

 Continued development

In future projects, I want to improve my understanding of:

* Responsive and mobile-first design
* CSS Flexbox
* CSS Grid
* The CSS box model
* Relative and absolute units
* Typography and spacing
* Accessibility and semantic HTML
* Writing cleaner and more maintainable CSS
* Designing layouts that adapt naturally to different screen sizes

I also want to become more comfortable deciding when fixed dimensions are appropriate and when flexible units such as `%`, `rem`, `em`, `vw`, and `vh` should be used.

 Useful resources

* [Frontend Mentor](https://www.frontendmentor.io/) - Used for the challenge design and project requirements.
* [MDN Web Docs](https://developer.mozilla.org/) - Used as a reference for HTML and CSS concepts.
* [Google Fonts](https://fonts.google.com/) - Used to explore fonts for the project.


 AI Collaboration

I used **ChatGPT** as a learning and debugging assistant while working on this project.

I mainly used it to:

* Understand CSS Flexbox concepts.
* Understand how `justify-content`, `align-items`, and `flex-direction` work.
* Debug the positioning of the footer.
* Understand how to center elements and text.
* Understand how to reference images stored inside an `images` folder.
* Learn how to import and apply Google Fonts.
* Understand CSS dimensions and the box model.
* Discuss whether a media query was necessary for the component.
* Clarify CSS concepts when the visual result was different from what I expected.

I used AI primarily to understand concepts and troubleshoot problems rather than having it build the entire project for me.

Author

Rinkesh Kumar Gope

Acknowledgments

Thanks to **Frontend Mentor** for providing realistic frontend challenges that help developers practice building projects from design specifications.

I also used ChatGPT as a learning companion to better understand CSS layout, Flexbox, dimensions, spacing, and debugging during the project.
