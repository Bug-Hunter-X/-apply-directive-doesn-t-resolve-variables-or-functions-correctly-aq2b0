# TailwindCSS @apply Directive Variable Resolution Bug

This repository demonstrates a bug where Tailwind's `@apply` directive fails to correctly resolve CSS custom properties (variables) or functions when applied within custom styles. 

## Bug Description
The `@apply` directive, when used with CSS variables or functions, does not correctly apply the computed values leading to unexpected styling or rendering errors.  This behavior is inconsistent across browsers and Tailwind versions.

## Reproduction
1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Compile your Tailwind styles.
4. Observe the unexpected styling in your application.

## Solution
The recommended solution is to avoid using variables or functions directly within `@apply` directives. Instead, define the styles with the resolved values or use standard Tailwind utility classes.

## License
MIT