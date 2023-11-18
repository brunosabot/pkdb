# Video

## Contents

- [Subtitles styles](#subtitles_styles)

## <a name="subtitles_styles"></a>Subtitles styles

Use the `::cue` pseudo selector.

You can add selector in parenthesis to target a specific selector in the subtitles

```css
::cue {
  color: #336699;
  background-color: #ffb010;
}

::cue(u) {
  text-decoration: underline;
  text-decoration-style: wavy;
  text-decoration-color: lightblue;
}

::cue(.custom-class) {
  font-family: Papyrus;
  color: khaki;
}
```
