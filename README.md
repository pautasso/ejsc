# EJS Compiler

Compile all `views/*.ejs` files into a single `/public/js/views.js` file.

## How to use

```bash
yarn run ejsc
```

## How to render the views on the browser

Include the generated views:

```html
    <script src="js/ejs.min.js"></script>
    <script src="js/views.js"></script>
```

Call the render function for each view `v`:

```js
dom.innerHTML = ejs.views_v({})
```

Yes, it supports includes out of the box.
