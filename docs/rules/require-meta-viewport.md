# require-meta-viewport

This rule enforces the use of `<meta name="viewport">` in the `<head>`.

## Why?

Different browsers and devices may have default viewport settings.
Including a `<meta name="viewport">` tag ensures a consistent and predictable layout across screen sizes and platforms.

## How to use

```js,.eslintrc.js
module.exports = {
  rules: {
    "@html-eslint/require-meta-viewport": "error",
  },
};
```

## Rule Details

Examples of **incorrect** code for this rule:

```html,incorrect
<html>
  <head></head>
</html>
```

Examples of **correct** code for this rule:

```html,correct
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
  </head>
</html>
```
