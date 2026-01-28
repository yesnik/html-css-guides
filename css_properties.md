# CSS Properties

## border

The `border` shorthand CSS property sets an element's border.

`border:`
- `1px solid red`
- `1rem dashed red` - dashed border
- `thick double #faf` - double border
- `10px ridge rgba(170, 50, 220, .6)` - ridge border

## margin

```css
html {
  margin: 0 auto;
}
```

The first value affects the element's top and bottom side, 
the second value affects the left and right side. 

`auto` is a special value that divides the available horizontal space evenly between left and right.

## text-decoration

The `text-decoration` shorthand CSS property sets the appearance of decorative lines on text. 

`text-decoration:`
- `underline` (default)
- `underline dotted red`
- `underline wavy blue`
- `underline overline wavy blue`

## transition

Change background color gradually on hover on and off:

```html
<button class="banner-btn">Hello</button>
```
```css
.banner-btn {
  text-decoration: none;
  background-color: var(--light);
  border: none;
  border-radius: 5px;

  transition: .2s;
}
.banner-btn:hover {
  background-color: var(--dark);
}
```
