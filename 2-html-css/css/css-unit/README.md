## CSS Unit

### Absolute Units

- bsolute units are fixed and do not change relative to other elements. They are usually based on physical measurements.

1. Pixels (px): Fixed unit, equal to one dot on the computer screen.

```css
.box {
  width: 100px;
  height: 50px;
}

```
- There are more fixed units like, `in, cm, mm, pt, pc`

### Relative Units

1. Percent (%): Relative to the parent element's size.

```css
.box {
  width: 50%;
}


```

2. Em (em):

- Relative to the font-size of the element's parent. If the parent font-size is 16px, 2em would be 32px.

```css
.text {
  font-size: 2em; /* twice the size of the parent font size */
}


```

3. Rem (rem):

- Relative to the font-size of the root element (<html>).

```css
:root {
  font-size: 16px;
}
.text {
  font-size: 2rem; /* 32px */
}


```

4. Viewport Width (vw):

- Relative to 1% of the viewport's width.

```css
.box {
  width: 50vw; /* 50% of the viewport width */
}

```

5. Viewport Height (vh):
- Relative to 1% of the viewport's height.

```css
.box {
  height: 50vh; /* 50% of the viewport height */
}


```

6. Viewport Minimum (vmin):

- Relative to 1% of the viewport's smaller dimension (width or height).

```css
.box {
  width: 10vmin; /* 10% of the smaller of the viewport's width or height */
}

```

7. Viewport Maximum (vmax):

- Relative to 1% of the viewport's larger dimension (width or height).

```css
.box {
  width: 10vmax; /* 10% of the larger of the viewport's width or height */
}

```

8. Viewport Size (svw, svh, lvw, lvh, dvw, dvh):

- These units relate to the size of the viewport, considering different scenarios like small viewport (svw, svh), large viewport (lvw, lvh), and dynamic viewport (dvw, dvh).

```css
.box {
  width: 50svw; /* 50% of the small viewport width */
  height: 50lvh; /* 50% of the large viewport height */
}

```