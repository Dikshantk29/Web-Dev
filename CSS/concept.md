# Concept of CSS (Cascading Style Sheets)

# Key Concepts of CSS:

1. **Selectors**: CSS uses selectors to target HTML elements. Common selectors include element selectors (e.g., `h1`, `p`), class selectors (e.g., `.class-name`), and ID selectors (e.g., `#id-name`).

2. **Properties and Values**: CSS rules consist of properties and values. For example, `color: red` sets the text color to red.

3. **Inheritance**: CSS allows you to inherit properties from parent elements. This is useful for creating consistent styles across different elements.

4. **Specificity**: CSS uses a priority system to determine which rules apply to a given element. Higher priority rules override lower priority rules.

5. **Box Model**: Every HTML element is represented as a rectangular box. The box model consists of margins, borders, padding, and the content area.

6. **Flexbox and Grid**: CSS provides layout models like Flexbox and Grid to create responsive and flexible layouts.

7. **Media Queries**: CSS allows you to apply styles based on the device's characteristics
   (e.g., screen size, orientation). This is essential for responsive design.

8. **Pseudo-classes and Pseudo-elements**: These are special selectors that allow you to style elements based on their state (e.g., `:hover`, `:focus`) or to target specific parts of an element (e.g., `::before`, `::after`).

9. **Transitions and Animations**: CSS can create smooth transitions and animations to enhance user experience.
10. **Comments**: CSS supports comments, which are ignored by the browser but can be useful for documentation. Comments are written as `/* comment */`.

# Example of a Simple CSS Rule:

```css
body {
  background-color: #f0f0f0;
  color: #333;
  font-family: Arial, sans-serif;
}

h1 {
  color: #007bff;
  text-align: center;
}
```

# class selectors

```html
<div class="header">
  <h1>Welcome to My Website</h1>
</div>
```

```css
.header {
  background-color: #f0f0f0;
  padding: 20px;
  text-align: center;
}
.header h1 {
  color: #333;
  font-size: 2em;
}
```

# ID selectors

```html
<div id="main-content">
  <p>This is the main content of the page.</p>
</div>
```

```css
#main-content {
  background-color: #ffffff;
  padding: 20px;
  border: 1px solid #ccc;
}
```

# Universal Selector

```html
<p>This is a paragraph.</p>
```

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

# Element Selector

```html
<p>This is a paragraph.</p>
```

```css
p {
  color: #333;
  font-size: 1em;
  line-height: 1.5;
}
```

# flexbox and text-align and align-items

```````html
<div class="container">
  <h1>Centered Heading</h1>
  <p>This paragraph is centered within the container.</p>
</div>
``````css .container { display: flex; flex-direction: column; align-items:
center; text-align: center; }
```````

## what is difference between align-items and text-align?

````
```align-items
- `align-items` is a Flexbox property that aligns flex items along the cross axis (vertically in this case). It affects the positioning of the child elements within the flex container.
- In the example, `align-items: center;` centers the heading and paragraph vertically within the container.

text-align
- `text-align` is a property that aligns inline content (like text) within a block container. It affects the horizontal alignment of text within its container.
- In the example, `text-align: center;` centers the text of the heading and paragraph horizontally within the container.
````

## css box model

```html
<div class="container">
  <div class="box">
    <p>This is a box model example.</p>
  </div>
</div>
```

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; /* Full viewport height */
}
.box {
  background-color: #ffffff;
  padding: 20px;
  border: 1px solid #ccc;
}
.box {
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  width: 300px; /* Fixed width */
  height: 200px; /* Fixed height */
}
```

# Display Property

diplay :none;

- The `display: none;` property hides an element from the page, removing it from the document flow. The element will not take up any space, and it will not be visible to the user.

diplay :block;

- The `display: block;` property makes an element a block-level element, meaning it will take up the full width available and start on a new line. Block-level elements can have width and height set, and they will stack vertically.

diplay :inline;

- The `display: inline;` property makes an element an inline element, meaning it will not start on a new line and will only take up as much width as necessary. Inline elements cannot have width or height set, and they will not break the flow of text.

## position Property

position: relative;

- The `position: relative;` property positions an element relative to its normal position in the document flow. It allows you to use the `top`, `right`, `bottom`, and `left` properties to adjust the element's position without affecting the layout of surrounding elements.

position: absolute;

- The `position: absolute;` property positions an element relative to its nearest positioned ancestor (element with a position other than `static`). If no such ancestor exists, it will be positioned relative to the initial containing block (usually the `<html>` element). The element is removed from the document flow, and it can overlap other elements.

position: fixed;

- The `position: fixed;` property positions an element relative to the viewport, meaning it will remain in the same position even when the user scrolls the page. It is useful for elements that should remain fixed on the screen, such as navigation bars or sidebars.

position: sticky;

## css units

1. **Absolute Units**: `px` (pixels), `cm`, `in`, `mm`, `pt`, `pc`.
   definition of px
   px: 1px = 1/96th of an inch

2. **Relative Units**: `em`, `rem`, `vw`, `vh`, `%`.
   defination of em and rem
   em: 1em = 1em of the parent element
   rem: 1rem = 1em of the root element

3. **Viewport Units**: `vh` (viewport height), `vw` (viewport width).

defination of vh and vw
vh: 1vh = 1% of the viewport height
vw: 1vw = 1% of the viewport width


# Most Important
## CSS FLEXBOX
https://css-tricks.com/snippets/css/a-guide-to-flexbox/

## CSS GRID
https://css-tricks.com/snippets/css/complete-guide-grid/#