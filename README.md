# Tourist Spot Page

## What I Learned (brief summary)

This project was developed as part of a Rocketseat challenge. The goal was to practice semantic HTML, structured content with headings and sections, and advanced CSS techniques using variables for consistent theming. I learned how to apply typographic hierarchy, create custom list counters, work with images using `object-fit`, and design dividers for clear content separation. Additionally, I reinforced the use of class selectors, ID selectors, pseudo-elements, and CSS custom properties for colors.

---

## Project Breakdown — What Was Used and Why

### HTML: structure and semantics

* `<!DOCTYPE html>`
  Enables HTML5 standard mode.
* `<html lang="pt-br">`
  Defines the language of the document.
* `<head>` with metadata and Google Fonts
  Loads fonts and sets responsive viewport.
* `<main>`
  Groups the main content of the page.
* `<header>`
  Introduces the page with subtitle and headline.
* `<section>`
  Used to organize related blocks of content (description, list of attractions).
* `<ol class="custom-list">`
  Ordered list for attractions, customized with CSS counters.
* `<ul>`
  Nested lists to describe highlights for each attraction.
* `<img src="..." alt="...">`
  Adds visual content with accessibility in mind.
* `<footer>`
  Contains credits and closes the document.

### CSS: concepts applied

* **CSS variables (`:root`)**
  Defined reusable values for colors such as `--background-default`, `--text-primary`, `--accent-blue`, etc.
* **Reset and box-sizing**
  `* { margin: 0; padding: 0; box-sizing: border-box; }` creates a consistent baseline.
* **Typography**
  Different font sizes and weights for `h1`, `h2`, `h3`, and paragraphs. Headings use strong hierarchy with uppercase and bold styles.
* **Images with `object-fit`**
  Ensures images adapt to containers without distortion.
* **Divider**
  A styled line (`.divider`) used to visually separate sections.
* **Custom list with counters**
  The ordered list increments a counter, and `::before` displays numbers before each title.
* **ID-based styles**
  Each list item (`#l1`, `#l2`, `#l3`, etc.) has a different accent color applied.
* **Pseudo-elements and markers**
  `::before` adds numbers to headings, and `::marker` customizes bullet colors.
* **Spacing and alignment**
  `margin`, `padding`, and `text-align` were used to create clear visual separation and centered text.

---

## Selectors and Combinations

### Basic selectors

* **Type selectors:** `body`, `h1`, `p`, `ul`, `footer`
* **Class selectors:** `.headline`, `.subtitle`, `.divider`, `.custom-list`, `.text-list`
* **ID selectors:** `#description`, `#final-text`, `#l1`, `#l2`, etc.

### Combinators

* **Descendant:** `header .headline` targets only `.headline` inside `header`.
* **Adjacent sibling (`+`):** `p + p` adds spacing only between consecutive paragraphs.

### Pseudo-elements and pseudo-classes

* `h3::before` adds the counter before each attraction title.
* `ul li::marker` customizes the bullet color.

---

## Learning Checklist

* [x] Semantic tags: `main`, `header`, `section`, `footer`, `h1`–`h3`, `p`, `ol`, `ul`, `li`, `img`
* [x] CSS variables for colors and theme consistency
* [x] Box model: `box-sizing`, `margin`, `padding`, `border-radius`
* [x] Typography hierarchy with headings and paragraphs
* [x] Images styled with `object-fit` and responsive sizes
* [x] Custom counters with `counter-increment` and `::before`
* [x] Pseudo-elements (`::before`, `::marker`) and sibling combinator (`+`)
* [x] Accessibility with `lang` attribute and `alt` text for images
