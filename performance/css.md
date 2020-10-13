# Perfomance

## Contents

- [Lazy offscreen draw](#lazy_offscreen_draw)

## <a name="lazy_offscreen_draw"></a>Lazy offscreen draw

`content-visibility` is a new property that tells the browser not to render the offscreen DOM elements

It makes the page load faster by preventing some heavy stuff to load such as images.

```css
.card {
  content-visibility: auto;
}
```
