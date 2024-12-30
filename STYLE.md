## Code Formatting

### Indentation
- Use **4 spaces** for indentation. Do not use tabs. (Except for in Makefiles)

### Whitespaces
- Use a single whitespace character between keywords like if, while, and for and the opening bracket to differentiate them visually from function calls.
- Opening brace `{` must be in the same line as function declaration, but closing brace `}` must be on a new line.
- No redundant whitespaces at the end of a line.
- No whitespaces at the start of a new scope (new functions, new loops, new conditionals)
- Use whitespaces to clearly seperate different blocks of code logic

### Line Length
- Limit lines to **100 characters**. If a line exceeds this limit, break it into multiple lines.

### Naming Conventions
- **Variables and Functions**: Use `camelCase`.
  - Example: `let userName = 'John';`
- **Constants**: Use `UPPER_SNAKE_CASE`.
  - Example: `const MAX_HEIGHT = 500;`
- **CSS Classes**: Use `kebab-case`.
  - Example: `.main-container {}`

### Comments
- Try to have code be obvious without the use of comments but use comments to explain non-obvious code or complex logic.
- Have javadoc style headers explaining functionality and usage of each function and class and any parameters passed or values returned.

## HTML Guidelines

- Use **lowercase** for element names, attributes, and values (except `DOCTYPE`).
- Use double quotes for attribute values.

### Example:
```html
<img src="image.jpg" alt="An example image">
```

## TypeScript Guidelines

### Variables and Constants
- Prefer `const` and `let` over `var`.
- Avoid global variables; keep everything scoped.

## CSS Guidelines

### Order of Rules
- Use the following order for CSS properties:
  1. **Positioning** (e.g., `position`, `top`, `right`, etc.)
  2. **Box Model** (e.g., `width`, `height`, `margin`, etc.)
  3. **Typography** (e.g., `font`, `text-align`, etc.)
  4. **Visual** (e.g., `background`, `border`, etc.)

### Example:
```css
.main-container {
  position: relative;
  width: 100%;
  margin: 0 auto;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
```

## Git Commit Messages

- Commit messages should be **concise and descriptive**.

## General Styling 

- For all other styling  methods follow the commonly accepted style guide for the language
 - When using Python Follow [PEP8](https://peps.python.org/pep-0008/)
 - When using Typescript Follow the [Google Typescript Style Guide](https://google.github.io/styleguide/tsguide.html)
