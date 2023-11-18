# CSS

## Contents

- [Automatic color ratio](#automatic_color_ratio)
- [Links](#links)

## <a name="automatic_color_ratio"></a>Automatic color ratio

Considering:

- The element as `--r`, `--v` and `--b` variables defining the background color

```css
.element {
  --l: calc(
    (
        1 / 2 -
          ((0.2126 * var(--r) + 0.7152 * var(--g) + 0.0722 * var(--b)) / 255)
      ) * 1000%
  );

  background-color: rgb(var(--r), var(--g), var(--b));
  color: hsl(0, 0%, var(--l));
}
```

## <a name="links"></a>Links

Always show the underline on a link, change thickness on hover

```css
a {
  text-decoration-line: underline;
  text-underline-offset: 0.25em;
  text-decoration-skip-ink: none;
}

a:hover {
  text-decoration-thickness: 3px;
}
```
