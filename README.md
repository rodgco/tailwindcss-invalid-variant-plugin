# Tailwind CSS Invalid Variant Plugin

The invalid CSS selector is usefull for highlighting input errors that requires user attention. With this plugin you can use the invalid variant selector with Tailwind as you normally do with the "hover" & "focus" selectors.

## Requirements

This plugin requires Tailwind CSS 1.2 or later.

## Installation

```bash
npm install tailwindcss-invalid-variant-plugin
```

or

```bash
yarn add tailwindcss-invalid-variant-plugin
```

## Usage

```js
// tailwind.config.js
module.exports = {
  variants: {
    backgroundColor: ["responsive", "hover", "focus", "invalid"],
    borderColor: ["responsive", "hover", "focus", "invalid"],
  },
  plugins: [require("tailwindcss-invalid-variant-plugin")],
};
```

Don't forget to include it in the variants you want to use. I'd recommend to take a look at the ones that already serve "hover" & "focus" variants.

Now you should be able to use it in your code, as any other pseudo-class.

```html
<input
  type="email"
  class="invalid:border-red-500 invalid:bg-red-100 invalid:border-t-2 p-1 bg-indigo-100 border-indigo-500 border-b-2 focus:outline-none"
/>
```

## CONTRIBUTING

- ⇄ Pull requests and ★ Stars are always welcome.
- For bugs and feature requests, please create an issue.
