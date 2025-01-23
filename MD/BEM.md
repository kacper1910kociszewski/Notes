
BEM (Block Element Modifier) is a methodology for organizing CSS to make it more readable, reusable, and maintainable. It uses a naming convention:

- **Block**: Represents a standalone component (e.g., `menu`).
- **Element**: A part of the block, tied to it (e.g., `menu__item`).
- **Modifier**: A variation or state of the block or element (e.g., `menu__item--active`).

#example 
>[!tag] HTML
```html
<div class="button button--primary">
  <span class="button__icon"></span>
  <span class="button__label">Click me</span>
</div>

```

>[!tag] CSS
```css
.button {
  display: inline-flex;
  align-items: center;
  padding: 10px 20px;
  border: none;
}

.button--primary {
  background-color: blue;
  color: white;
}

.button__icon {
  margin-right: 5px;
}

.button__label {
  font-size: 16px;
}

```