# Position elements

`position:`
- `static` (default)
- `relative`
- `absolute` - we can set `position: relative` to a parent block and place the current block within it
- `fixed`
- `sticky`

## Center vertically

```css
.slick-btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}
```

## Button "Scroll up"

We can place a button in the right bottom corner that will be there during scroll:

```css
.btn-up {
  position: fixed;
  right: 30px;
  bottom: 30px;
}
```
