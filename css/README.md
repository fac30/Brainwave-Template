# Style Documentation

### Explanation of the CSS Structure

- **`/base`**: Contains base styles such as resets and typography settings. This is where you place styles that affect global elements (e.g., `body`, `a`, `h1`).
- **`/components`**: Contains styles specific to reusable components (buttons, cards, etc.).
- **`/layout`**: Contains layout-related styles such as grid, header, footer, and other layout elements.
- **`/pages`**: Contains page-specific styles. These are styles that apply only to a specific page (e.g., `home.css`, `about.css`).

### CSS Reset

A CSS reset helps standardize the styling across different browsers by removing default browser styles. A popular reset stylesheet is [Eric Meyer's Reset CSS](https://meyerweb.com/eric/tools/css/reset/), but you can also use a minimal reset or normalize CSS.

#### Example Reset CSS (`reset.css`)

Here’s a basic CSS reset to get started:

```css
/* reset.css */
/* Reset CSS by Eric Meyer v2.0 */
/* https://meyerweb.com/eric/tools/css/reset/ */
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
    display: block;
}
body {
    line-height: 1;
}
ol, ul {
    list-style: none;
}
blockquote, q {
    quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
    content: '';
    content: none;
}
table {
    border-collapse: collapse;
    border-spacing: 0;
}
```

### Best Practices for CSS

1. **Organize by Functionality**: Structure your CSS files by their purpose (e.g., base styles, components, layout) for better maintainability.
2. **Use a Reset or Normalize**: Apply a CSS reset or normalize to ensure consistency across different browsers.
3. **Follow a Naming Convention**: Use BEM (Block Element Modifier) or other naming conventions to keep your CSS readable and modular.
4. **Use Variables for Reusability**: Leverage CSS variables (custom properties) or a preprocessor (like SASS) for colors, spacing, and font sizes.
5. **Keep it Modular**: Break your CSS into smaller files/modules, making it easier to maintain and scale.
6. **Minimize Specificity**: Avoid deep nested selectors to keep specificity low and your CSS easier to override.
7. **Utilize Utility Classes**: Create reusable utility classes for common styles (e.g., `.m-1` for margin).

### Example of Combining Everything

**Root CSS (`root.css`):**

```css
/* Import Reset and Base Styles */
@import url('./reset.css');
@import url('./typography.css');

/* Global Styles */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f5f5f5;
}
```

With this structure, your CSS files will be easier to manage and scale as your project grows!