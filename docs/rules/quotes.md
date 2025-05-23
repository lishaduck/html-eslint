# quotes

This rule enforces enforces consistent use of quotes for attribute values (`'` or `"`).

## How to use

```js,.eslintrc.js
module.exports = {
  rules: {
    "@html-eslint/quotes": "error",
  },
};
```

## Rule Details

### Options

This rule has two options

- `"double"` (default): Requires the use of double quotes(`"`).
- `"single"`: Requires the use of single quotes(`'`)

#### "double"

Examples of **incorrect** code for this rule with the default `"double"` option:

<!-- prettier-ignore -->
```html,incorrect
<div id='foo'></div>
```

Examples of **correct** code for this rule with the default `"double"` option:

```html,correct
<div id="foo"></div>
<div id='containing "double" quotes'></div>
```

#### "single"

Examples of **incorrect** code for this rule with the `"single"` option:

```html,incorrect
<div id="foo"></div>
```

Examples of **correct** code for this rule with the default `"single"` option:

<!-- prettier-ignore -->
```html,correct
<div id='foo'></div>
<div id="containing 'single' quotes"></div>
```

## Further Reading

- [MDN - Quoting attributes](https://developer.mozilla.org/en-US/docs/MDN/Guidelines/Code_guidelines/HTML#Quoting_attributes)
