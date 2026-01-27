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
