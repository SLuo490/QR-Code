# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - QR code component solution](#frontend-mentor---qr-code-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
    - [Built with](#built-with)
  - [Documentation](#documentation)
    - [HTML](#html)
    - [Style](#style)
      - [Centering the body](#centering-the-body)
      - [Styling the image and sizing the container](#styling-the-image-and-sizing-the-container)
      - [Styling text](#styling-text)
  - [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![]()

### Links

- Solution URL: [Add solution URL here]()
- Live Site URL: [Add live site URL here]()

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

[Link to Project](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H)

## Documentation

### HTML

```html
<body>
  <main>
    <section>
      <img src="/images/image-qr-code.png" alt="" />
    </section>
    <section>
      <h1>Improve your front-end skills by building projects</h1>
      <h3>
        Scan the QR code to visit Frontend Mentor and take your coding skills to
        the next level
      </h3>
    </section>
  </main>
</body>
```

To follow HTML best practices, I used [semantic elements](https://www.w3schools.com/html/html5_semantic_elements.asp) instead of `div`.

### Style

#### Centering the body

```css
body {
  background-color: var(--light-gray);

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  height: 100vh;
}
```

`flex-direction` changes the direction of the content from row to column or vise versa. By doing `flex-direction: column;` I changed the direction of the content from being horizontal to being vertical.

The key point to make the content center vertically is making the body of the `height: 100vh`. If we didn't have this line, then the content wouldn't be centered, since the body does not cover the entire page.

#### Styling the image and sizing the container

```css
main {
  background: var(--white);
  width: 320px;
  height: 497px;

  display: flex;
  flex-direction: column;
  align-items: center;

  border-radius: 20px;
}

img {
  width: 288px;
  height: 288px;
  border-radius: 20px;
}

.image {
  margin: 16px 16px 24px 16px;
}
```

I added a `display: flex` to the container to make the image and the text center of the container. I made sure not to add `justify-content: center` because I don't want the content to be in the very center of the container.

Using the provided figma file, I added the pixels for both the image size and the container size to match the design. Adding `320` and `497` to the width and height of the container and `288` for both the width and height of the image. I also added border-radius to both the container and the image.

#### Styling text

```css
.text {
  text-align: center;
}

.heading {
  margin: 0px 16px;
  color: var(--dark-blue);
  font-weight: 700;
  font-size: 22px;
}

.details {
  margin: 16px 32px 40px 32px;
  color: var(--grayish-blue);
  font-weight: 400;
  font-size: 15px;
  letter-spacing: 0.188px;
}
```

Similar to the last step, I added styling to the text matching the design in figma. These steps were self explanatory as I copied the numbers from the design to the css.

## Author

- Website - [Shi Tao Luo](https://github.com/SLuo490)
- Frontend Mentor - [@qxer](https://www.frontendmentor.io/profile/SLuo490)
