# CSS

On todays lesson we have learned about:

- The box model
- Advanced CSS selectors
- Responsive design
- Flexbox
- Units

## Main concepts

### The box model:

- Content
- Padding
- Border
- Margin
- Reset the default margin, pading and box-sizing

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

### Advanced CSS selectors:

- Direct descendant selector

```css
.parent > .child {
  /* styles */
}
```

- Child selector (all children)

```css
.parent .child {
  /* styles */
}
```

- Adjacent sibling selector

```css
.element + .element {
  /* styles */
}
```

- Multiple selectors

```css
.element,
.element {
  /* styles */
}
```

### Responsive design:

#### Media queries
- Screens less than 768px:
```css
@media (max-width: 768px) {
  /* styles */
}
```

- Screens between 768px and 1024px:
```css
@media (min-width: 768px) and (max-width: 1024px) {
  /* styles */
}
```

- Screens greater than 1024px:
```css
@media (min-width: 1024px) {
  /* styles */
}
```

### Flexbox:

- Flex container: The parent element that contains the flex items we want to align.
- Flex items: The children of the flex container.

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```
Remember to add the flex property to the container and the flex items will be aligned.

### Units:
- Absolute units: px
- Relative units: em, rem, vw, vh, %

#### rem:
- Relative to the font-size of the root element (we saw in chrome dev tools that the root element has by default 16px font-size, so 1rem is equal to 16px)

#### em:
- Relative to the font-size of the element (2em means 2 times the size of the current font-size). For example: if the parent element has a font-size of 20px, 2em will be 40px.

#### vw:
- Relative to 1% of the width of the viewport. 100vw is equal to 100% of the viewport width.

#### vh:
- Relative to 1% of the height of the viewport. 100vh is equal to 100% of the viewport height.

#### %:
- Relative to the parent element. If the parent element has a width of 200px and the child element has a width of 50%, the child element will have a width of 100px.

