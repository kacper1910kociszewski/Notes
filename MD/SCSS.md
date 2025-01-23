---

---
**SCSS** (Sassy CSS) is a syntax of **Sass**, a preprocessor that extends CSS with additional features to make writing styles easier and more efficient. SCSS is fully compatible with regular CSS but introduces features like variables, nesting, mixins, inheritance, and more.

#variables
just fancy variables
```scss
$primary-color: blue; 
$padding: 10px; 
button { 
	background-color: $primary-color; 
	padding: $padding; 
} 
```

#nesting
Write CSS in a hierarchical way that matches your HTML structure.
```scss
nav {
  ul {
    list-style: none;
    li {
      display: inline-block;
      a {
        text-decoration: none;
      }
    }
  }
}

```

#mixins
Reuse blocks of CSS with optional arguments.
```scss
@mixin button-style($bg-color) {
  background-color: $bg-color;
  border: none;
  padding: 10px 20px;
}

.primary-button {
  @include button-style(blue);
}

```

#inharitance_extend
Share styles between selectors.
```scss
%shared-styles {
  font-family: Arial, sans-serif;
  color: black;
}

h1 {
  @extend %shared-styles;
}

p {
  @extend %shared-styles;
}

```

#Math_and_Functions
Perform calculations directly in your styles.
```scss
$base-spacing: 8px;

div {
  margin: $base-spacing * 2; // 16px
  width: 100% / 3;          // 33.33%
}

```

#Partials_and_Imports
Break CSS into smaller files and import them as needed.
```scss
// _variables.scss
$primary-color: blue;

// main.scss
@import 'variables';

body {
  background-color: $primary-color;
}

```

#expample_of_usage_with_bem
SCSS features in BEM:
```scss
// Block
.button {
  padding: 10px 20px;
  border: none;

  // Element
  &__icon {
    margin-right: 5px;
  }

  &__label {
    font-size: 16px;
  }

  // Modifier
  &--primary {
    background-color: blue;
    color: white;
  }
}

```

#how_to_install
### For Visual Studio Code:
To use scss in thy VSCode project you need just install extension called "`Live SASS Compiler`", then create file `.scss`, finally in bottom of VSCode window u will be able to find "`Watch Sass`" button, which one you need to click. All Done.
![[Pasted image 20250122160145.png]]
### For other editors:
For other editors (ex. Vim) you can install ruby, in the guide below you will find everything u need to do so


#Links
## Links: 
>Install Guide:
	https://www.youtube.com/watch?v=Do7ivdaQU8Y
>Ruby:
	https://rubyinstaller.org/downloads/



