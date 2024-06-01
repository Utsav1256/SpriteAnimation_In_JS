# SpriteAnimation_In_JS

# Whole process explained ;)

## Creating a canvas element and getting its reference in script.js

- We have to create an canvas element in the `index.html`

```html
<body>
  <canvas id="canvas1"></canvas>
  <!-- it will serve as our drawing board  -->

  <script src="./script.js"></script>
</body>
```

- it will serve as the drawing board for us.

- we will draw our animation on this canvas.

- Now, we will get the reference of this `<canvas>` element in our `script.js` file.

```js
const canvas = document.getElementById("canvas1");
```

- How it works??

-- `document` is a global object that represents the entire HTML document.

-- `getElementById()` is a method that returns the element with the specified id.

-- In this case, it returns the `<canvas>` element whose id is canvas1.

-- `const` is used to declare a constant variable named canvas that holds the reference to this `<canvas>` element.

## Get the rendering context for the `<canvas>` element

- The `rendering context` is an `object` that provides `methods and properties` for drawing and manipulating the content on the canvas.

```js
const ctx = canvas.getContext("2d");
```

- How it works??

-- `canvas` is the variable holding the reference to the `<canvas>` element (obtained in the previous line).

-- `getContext` is a method of the `<canvas>` element that returns a drawing context on the canvas.

-- The argument `"2d"` specifies that you want to get a `2D rendering context`. This is the context type used for drawing `2D graphics`.

-- When you call `canvas.getContext("2d")`, it returns a `2D rendering context object` that allows you to `draw and manipulate content` on the canvas. This context is your main tool for drawing shapes, text, images, and other graphics.
