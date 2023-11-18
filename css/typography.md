# Typography

## Contents

- [Fluid font-size](#fluid_font_size)

## <a name="fluid_font_size"></a>Fluid font-size

Use the clamp function, which takes 3 parameters

```css
.title1 {
  font-size: clamp(1rem, calc(5vw + 1rem), 5rem);
}
.title2 {
  font-size: clamp(1rem, 5vw + 1rem, 5rem);
}
```
